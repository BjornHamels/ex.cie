# Aanvraag externe minor
Zie [de beleidswiki](https://beleidswiki.fhict.nl/doku.php?id=beleid:minoren), in het gehele minorproces zit de toestemming voor het volgen van een minor relatief laat in het process.
Deze aanvragen worden behandeld door Examenkamer D.
Grofweg zijn deze aanvragen op te delen in externe minors in Nederland en daarbuiten.

## Doel
De ex.cie ziet er op toe dat er geen significante overlap zit in de al eerder "uitbetaalde" ECTS. De student is vrij om een minor te kiezen die geaccrediteerd 30 ECTS uitbetaald in een post-propedeuse onderwerp.

## Terminologie
| Term | Beschrijving |
| --- | --- |
| LA | Learning Agreement, document waarop de ex.cie haar handtekening zet ter goedkeuring. |
| Kiesopmaat | Kiestopmaat is [een website](https://kiesopmaat.nl) waarop samenwerkende hogescholen en universiteiten hum minors publiceren. Minors die door studenten op die site gekozen worden worden onderling gefactueerd en zijn standaard voorzien van LA's en modulebeschrijvingen. |
| Opleidingsminor | Minor waarbij de doorstroom ingeregeld is via het OER/ opleidingsgids. Toestemming aanvragen bij de ex.cie is hierdoor niet nodig. |
| Fontys-minor | Fontys-breede minor waarbij de doorstroom ingeregeld is via het OER/ opleidingsgids. Toestemming aanvragen bij de ex.cie is niet nodig. |
| Schakelminor | Minor (pre-master) waarbij de doorstroom ingeregeld is via het OER/ opleidingsgids. Toestemming aanvragen bij de ex.cie is niet nodig. |
| Externe minor | Minor waarbij de ex.cie toestemming moet geven. Dit bestand richt zich op de procedure omtrent dit type minor. |



## Procedure externe minor in Nederland
Deze procedure richt zich op de aanvraag voor een externe minor in Nederland.


```mermaid
---
title: Ex.cie aanvraag externe minor Nederland
---
flowchart TD

    %% Start
    Start((Start))-->TypeM
    TypeM{Type minor?}-->|Binnen Nederland|NL{Kiesopmaat?}
    
    %% Kiesopmaat
    NL-->|Ja, gebruik
      meegeleverde LA en
    modulenoverzicht|CtrlOver{Controle
      significante
      overlap}
    TypeM-->|Buiten Nederland|Buitenland[[Zie ex.cie aanvraag
      minor buitenland]]
    NL-->|Nee|NLNietKies{Geaccrediteerd?
      30 ECTS?}

    %% 30 ECTS?
    NLNietKies-->|Ja|GeAcc{Onderzoek
      kosten}
    NLNietKies-->|Nee|Geen30((Afwijzen))

    %% De bronnen van Controle overlap
    SVS[(SVS)]-->|Behaalde
      semesters|CtrlOver
    DOC[/Docent/].->|Quick check
      bij collega|CtrlOver
    CE[/CE/].->|Escalatie
      check|CtrlOver
    STU[/Student/].->|Opvragen PP /
      opvragen motivatie|CtrlOver

    %% Na Controle significante overlap
    CtrlOver-->|Geen
      significante
      overlap|Tekenen[Tekenen]
    Tekenen-->|Versturen naar
      student|Student((Ex.cie tool))
    CtrlOver-->|Significante
      overlap
      aanwezig|Afwijzen((Afwijzen))
    Afwijzen-.->|Reparatie|CtrlOver

    %% Indien geen kiesopmaat
    SC[/SC/].->|Overleg SC|GeAcc
    Voorzitter[/Voorzitter/]-->|2bd opinion
      voorzitter|GeAcc
    FZ[/FZ/]-->|Intentie
      betaling
      opvragen|GeAcc
    GeAcc-->|Kosten ok,
      budg.nr.|MaakLA[Stel
      LA op]
    STU2[/Student/]-->|Produceert het
      grootste deel
      van de LA|MaakLA
    MaakLA-->|Tijdens/ vervolg
      het proces|CtrlOver
    GeAcc-->|Te duur|TeDuur((Afwijzen))

```
