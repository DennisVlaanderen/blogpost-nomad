# Nomad: multi-region deployments, voor mensen die niet van stress houden

*Dennis Vlaanderen*, oktober 2023
<img src="./resources/Nomad_PrimaryLogo_FullColor.png" width="200" align="right">

---

Voor ontwikkelaars die zich bezighouden met schaalbare software-implementaties, is de wereld van DevOps vol met uitdagingen en mogelijkheden.
Het beheersen van de kunst van efficiënte multi-region deployments is een cruciaal aspect geworden in de snel evoluerende digitale landschappen van vandaag.

In deze complexe wereld van gedistribueerde systemen en geografisch verspreide gebruikers, komt Nomad naar voren als een krachtige en betrouwbare gids.
Deze blogpost werpt een licht op de cruciale rol die Nomad speelt in het vereenvoudigen van multi-region deployments.
Of je nu een ervaren ontwikkelaar bent die zoekt naar nieuwe manieren om wereldwijd schaalbare applicaties te implementeren, of een nieuwkomer die geïnteresseerd is in de mogelijkheden van DevOps, deze post biedt concrete inzichten en praktische toepassingen.

We duiken dieper in de wereld van multi-region deployments en laten zien hoe Nomad het mogelijk maakt om naadloos tussen verschillende regio's te schakelen.
Met Nomad kunnen ontwikkelaars hun applicaties effectief verdelen over diverse geografische locaties, met behoud van consistentie en betrouwbaarheid.

## Wijdverspreide beschikbaarheid

Multi-region deployments zijn een geavanceerde DevOps-praktijk waarbij softwareapplicaties en services worden uitgerold over meerdere geografische locaties. Dit stelt bedrijven in staat om hun toepassingen wereldwijd beschikbaar te maken, waardoor ze kunnen profiteren van lagere latentie, verbeterde betrouwbaarheid en gegevensbescherming. Met deze aanpak kunnen organisaties hun gebruikers bedienen vanuit de dichtstbijzijnde serverlocatie, wat resulteert in een naadloze gebruikerservaring, zelfs in verschillende delen van de wereld. (Goldman, 2022)

## Deployen van microservices

Container orchestration is het kloppende hart van moderne softwarearchitectuur. Het biedt een georganiseerd, efficiënt en schaalbaar systeem voor het beheren van containers, de draagbare eenheden waarin applicaties en hun afhankelijkheden zijn verpakt. In de complexe wereld van hedendaagse IT, waar flexibiliteit en snelheid essentieel zijn, biedt container orchestration een gestroomlijnde methode om applicaties te implementeren, te schalen en te beheren. Door automatisering van cruciale taken zoals load balancing, failover en resourcebeheer, stelt container orchestration teams in staat zich te concentreren op innovatie in plaats van zich zorgen te maken over de operationele complexiteit. Het verhoogt niet alleen de operationele efficiëntie maar versnelt ook de ontwikkeltijd, waardoor bedrijven wendbaarder en concurrerender worden in de dynamische digitale markt. (Mitra & Nadareishvili, 2020) Daarnaast verbeterd het ook de mogelijkheid tot ophalen van specifieke metrics door opsplitsing van kleine individuele services in plaats van één grote applicatie.

<img src="./resources/disk_usage.png" alt="xkcd over Disk Usage">

*Figuur 1*: Resource Management in handen van gebruikers

## Bouwstenen van Nomad

Nomad, HashiCorp's veelzijdige orchestratiesysteem, steunt op essentiële elementen voor naadloze multi-region deployments. Met de 'Job Specification' definieer je taken, terwijl 'Nodes' fysieke/virtuele machines vertegenwoordigen waarop taken draaien. 'Regions' beheren geografische afstanden, terwijl 'Schedulers' intelligent taken verdelen onder deze Regions. 'Federation' laat clusters wereldwijd samenwerken, terwijl netwerkintegratie en monitoring cruciaal zijn voor naadloze communicatie en prestatiemonitoring. Nomad biedt ook een robuuste API en CLI voor beheer, wat ontwikkelaars en operators in staat stelt om Nomad-gebaseerde implementaties moeiteloos te beheren, ongeacht hun locatie. Deze bouwstenen vormen de ruggengraat van Nomad's mogelijkheid om complexe wereldwijde implementaties te realiseren.

<img src="./resources/Nomad_architecture.png" alt="Basis architectuur nomad">

*Figuur 2*: Basis-architectuur Nomad

## 

## Bronnen

Goldman, M. (2022, 1 september). 5 reasons to build multi-region application architecture. *Cockroach Labs*.  
Geraadpleegd op 3 oktober 2023, van https://www.cockroachlabs.com/blog/5-reasons-to-build-multi-region-application-architecture/

Mitra, R., & Nadareishvili, I. (2020). Microservices: up and running: A Step-By-Step Guide to Building a Microservice Architecture. O’Reilly Media.
