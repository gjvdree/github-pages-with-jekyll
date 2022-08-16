---
title: "Energie Inzicht"
date: 2022-07-14
---
# Grip op je energie

### Dev
De developer in mij wil graag alles automatiseren, want waarom een kleine taak doen in een paar minuten als je er uren aan kan besteden om het te automatiseren. Fröbelen met techniek is nu eenmaal een hobby waar ik energie uit haal. Met de stijgende gasprijzen, omvallende energiemaatschappijen en een klimaatcrisis kan een extra kritische blik op de energieconsumptie zeker geen kwaad. In dit blog vertel ik je hoe ik meer inzicht in het energieverbruik heb gekregen.

### RPi (Raspberry Pi)
<img align="right" width="20%" src="../images/2022-07-14-Energy_Insights/image001.jpg">
Ergens op zolder lag nog een raspberry Pi stof te vergaren. Een raspberry Pi is een minicomputer ter grootte van een creditcard met een legio aan mogelijkheden. Niet om windows op te draaien, want daar is hij niet krachtig genoeg voor, maar voor een leuk hobby projectje zijn ze perfect. Ze kosten een paar tientjes en gebruiken weinig stroom. Je zou er een mediaserver op kunnen draaien, of van die oude usb stick een netwerkschijf kunnen maken. Een collega heeft zelfs zijn brievenbus zo slim gemaakt dat hij weet wanneer de postbode is geweest. Ik gebruik hem om er HomeAssistant op te draaien voor home automation.

### Home Assistant
Home Assistant is een gratis en open source domotica systeem met de focus op privacy en controle.
Het is een centraal systeem waarmee je de status van slimme apparaten kan bijhouden, en kan aansturen. Je kan je slimme lampen aansturen of zelfs de airco van je auto aanzetten als de wekker gaat. 

### Watt?
<img align="right" width="20%" src="../images/2022-07-14-Energy_Insights/image002.png">
De eerste stap die ik gezet heb is het uitlezen van de zonnepanelen. Daar heb je toch gewoon een app voor zou je denken, en die is er inderdaad ook. Het nadeel van zo’n app is dat je in die app alleen de informatie van de zonnepanelen ziet, en niet van je slimme meter of het laadschema van je elektrische auto. Dat kan dus handiger. Met een kleine investering is het mogelijk om een P1 poort van de slimme energie meter uit te lezen. Zo krijg je ook inzicht in de energie die je afneemt van en terug levert aan het net. 


### Dashboard
<img align="left" width="20%" src="../images/2022-07-14-Energy_Insights/image003.png">
HomeAssistant heeft sinds eind 2021 een mooi dashboard waar alle informatie op samen komt. Je kan direct inzien wanneer je stroom afneemt, opwekt en terug levert. Met deze informatie kan je zien hoeveel eigen opgewekte stroom je gebruikt. Het geeft je inzicht in de hoeveelheid gas die je verbruikt en je zou op basis van deze informatie je verbruik aan kunnen passen om energie en geld te besparen.

### Installatie
<img align="right" width="20%" src="../images/2022-07-14-Energy_Insights/image004.png">
Het installeren van HomeAssistant op de raspberry Pi is vrij eenvoudig. Op home-assistant.io staat een stappenplan met de benodigde tools om snel aan de slag te kunnen. De volgende stap is het uitlezen van de zonnepanelen. Hoe dit precies met zal per installatie verschillen. Gelukkig is er voor onze zonnepanelen een kant en klare integratie beschikbaar.
<img align="left" width="20%" src="../images/2022-07-14-Energy_Insights/image005.png">
 In HomeAssistant is het eenvoudig om de integratie te vinden en door de stappen heen te lopen. Als de integratie klaar is dan is Enphase Envoy terug te vinden tussen de apparaten in HomeAssistant. De verschillende sensoren die de integratie biedt kunnen direct aan het dashboard toegevoegd worden, maar het energy dashboard van HomeAssistant heeft een veel betere grafische weergave. Om het energy dashboard te gebruiken moet het een en ander ingesteld worden. Gelukkig is de interface vrij eenvoudig en er staan meerdere links naar hulpdocumentatie.

### Meten is weten
<img align="left" width="20%" src="../images/2022-07-14-Energy_Insights/image006.png">
Wanneer de configuratie voltooid is verschijnen er een aantal mooie diagrammen op het energy dashboard. 
Een hele interessante is de hoeveelheid zelfopgewekte stroom die verbruikt wordt. In combinatie met de hoeveelheid stroom die afgenomen wordt van het net. Met die informatie kan het nut van een thuisbatterij goed in beeld worden gebracht. Vooral omdat het verschil tussen het teruglevertarief en energietarief behoorlijk is op het moment dat salderen niet meer mogelijk is. 

### Next
<img align="left" width="20%" src="../images/2022-07-14-Energy_Insights/image007.png">
En nu? We hebben meer inzicht in het energieverbruik, en kunnen zelfs bepalen wanneer sommige apparaten het beste aan kunnen staan. Overdag leveren de zonnepanelen genoeg stroom om de vaatwasser en de wasmachine te kunnen voorzien van stroom, overdag zouden deze apparaten dus het beste aan kunnen staan. 
Een volgende stap zou het toevoegen van lampen kunnen zijn, losse apparaten via slimme stekkers, of is misschien de investering van een thuisbatterij toch de moeite waard? 
