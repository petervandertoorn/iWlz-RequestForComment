![header](../imagesrc/ZinBanner.png "template_header")

# RFC0020 - Verwijsindex & Cooperative Search

<font size="4">**SAMENVATTING**</font>

**Huidige situatie:**

>```nog invullen```

**Beoogde situatie**

>```nog invullen```


<font size="4">**Status RFC**</font>

Volg deze [link](https://github.com/iStandaarden/iWlz-RFC/issues/19) om de actuele status van deze RFC te bekijken.

---
**Inhoudsopgave**
- [RFC0020 - Verwijsindex \& Cooperative Search](#rfc0020---verwijsindex--cooperative-search)
- [1. Inleiding](#1-inleiding)
  - [1.1. Uitgangspunten](#11-uitgangspunten)
  - [1.2 Relatie andere RFC](#12-relatie-andere-rfc)
- [2. Terminologie](#2-terminologie)
- [plant-uml embedding](#plant-uml-embedding)

---
# 1. Inleiding
In het verlengde van de Wegiz is een aantal generieke functies benoemd die de (verplichte) digitale uitwisseling van gezondheidsgegevens zullen ondersteunen. 
De NEN 7519 behandelt de generieke functie lokalisatie: het bepalen waar welke gegevens van de patiënt of cliënt zijn. NEN 7519 beschrijft de lokalisatiefunctie voor zorgverlening aan een individuele patiënt voor zowel primaire als secundair gebruik van de gegevens. Via een AMvB zal NEN7519 verplicht gesteld voor gegevensuitwisselingen binnen de Wegiz.

De norm behandelt een aantal use cases waarvoor de lokalisatie van de gezondheidsgegevens van de client noodzakelijk is. Deze use cases lijken ook op de functionele vragen die binnen de Wlz zullen ontstaan om de Wlz gegevens. Ook introduceert de norm de begrippen LDS (Lokaliseerbare dataset) en Lokalisatiestructuur 
dossierhouder maakt door lokalisatiestructuur (dataset die gedeeld kan worden tussen zorgverleners om gegevens vindbaar te maken). 

Het doel van de norm is de uitwisseling van lokalisatie-informatie op een uniforme manier, onafhankelijk van het systeem dat voor opslag of uitwisseling van de lokalisatie-informatie elektronische wijze mogelijk te maken.

In RFC0020 hebben wij de Verwijsindex en het mechanisme Cooperative Search geïntroduceerd. Het lijkt ons wenselijk de behoefte om iWlz gegevens van een client te vinden in een netwerk op dezelfde wijze op te lossen als dat NEN7519 dat voor de Wegiz voorstelt. Dat betekent dat:
•	de iWlz-gegevenssets als LDS gedefinieerd moeten worden;
•	voor de set een invulling van de lokalisatiestructuur bepaald moet worden;
•	procesmatige spelregels die de NEN7519 geeft gevolgd moeten worden;
•	autorisatieregels voor het delen van de lokatiestructuren uitgewerkt moeten worden.

De NEN 7519 laat in het midden hoe de locatiestructuren gedeeld worden door de bronhouders en hoe in lokalisatiestructuren naar de LDS gezocht wordt. Daar moeten we de inrichting voor uitdenken. Dit kan zowel via een (centrale) verwijsindex of via mechanisme als coöperatief zoeken.  Bronhouders zullen de iWlz-gegevens lokaliseerbaar moeten maken:
-	het vullen en onderhouden van de structuur; 
-	antwoord geven op een bevraging (‘deze endpoints’ of ‘deze zorgaanbieders’).
-	Logging bijhouden van de uitgewisselde lokalisatiestructuren 

In deze RFC zullen we de mechanismen voor het lokaliseerbaar maken van de gegevens en voor het vinden van de datasets uitwerken binnen de topologie van het iWlz-netwerk. Op basis daarvan stellen we vast welke functionaliteit bronhouders en afnemers daarvoor dienen te realiseren.

![image](https://github.com/user-attachments/assets/b4e549f2-296c-4e77-9e05-58a27c133f84)


## 1.1. Uitgangspunten
>```nog invullen```

## 1.2 Relatie andere RFC
Deze RFC heeft een relatie met de volgende RFC(s)
|RFC | onderwerp | relatie<sup>*</sup> | toelichting |issue |
|:--|:--|:--| :--|:--|
|[0008](RFC/RFC0008%20-%20Notificaties%20en%20Abonnementen.md) | Notificaties en abonnement | voorwaardelijk | <ul><li>Er is een **Service Directory** waarin notificatietypen gepubliceerd kunnen worden.</li> <li>Netwerkdeelnemers raadplegen de **Service Directory** om op te halen welke abonnementen geplaatst kunnen worden en welke voorwaarden hier aan zitten. </li></ul>|[#2](https://github.com/iStandaarden/iWlz-RFC/issues/2) |

<sup>*</sup>voorwaardelijk, *voor andere RFC* / afhankelijk, *van andere RFC*


# 2. Terminologie
Opsomming van de in dit document gebruikte termen.

| Terminologie | Omschrijving |
| :-------- | :-------- | 
| *term* | *beschrijving/uitleg* | 

# plant-uml embedding
Neem een verwijzing op naar het gegenereerde diagram
 ```
    ![notificatie_melding](../plantUMLsrc/rfc008-01-notificatie_melding.svg "notificatie_melding")
```

verberg de plant-Uml source tussen de tags: 

    <details>
     <summary>plantUML-source</summary>
    
     ```plantuml
     @startuml rfc008-01-notificatie_melding
     <plant-uml-source> 
     
    ```
     </details>
