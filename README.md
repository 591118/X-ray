Chest X-ray
==============================

## Introduksjon

Prosjektet undersøker deep learning modeller for å utforske x-ray av overkroppen, for å finne avvik fra en frisk kropp. Skal deretter sette riktig diagnose på avvikene.
Prosjektgruppen består av Håkon Mydland, Georg Taklo Kvalsund og Even Torbjørnsen. 
Målet for prosjektet var å lage et system som kan finne en eller mer av 14 tilstander fra et eller flere x-ray bilder. Utforske og integrere teknikker for “Explainable AI".
Prosjektet er en del av DAT255, og et ledd av vår bachelorgrad ved HVL innenfor dataingeniør/informatikk. 

Medisinsk bildeanalyse har lenge vært en essensiell komponent i moderne helsetjenester, og
røntgenbilder utgjør en stor del av dette feltet. Radiologer er avhengige av å kunne tolke disse bildene nøyaktig og effektivt for å kunne stille korrekte diagnoser og sikre optimal behandling for pasientene. Imidlertid kan manuell gjennomgang av røntgenbilder være tidkrevende og utsatt for menneskelige feil. I den forbindelse har det vokst fram et behov for å utvikle mer avanserte og automatiserte verktøy som kan bistå radiologer i deres arbeid. Dette prosjektet har som mål å utvikle en deep-learning basert modell som kan identifisere 14 ulike diagnoser gitt en eller flere røntgenbilder.

## Bakgrunn

Røntgenbilder har vært en essensiell komponent innen medisinsk diagnostikk siden oppdagelsen av røntgenstråler av Wilhelm Conrad Röntgen i 1895. Til tross for fremskritt innen andre bildeteknikker som computertomografi (CT), magnetisk resonansavbildning (MRI) og ultralyd, forblir røntgenbilder en rask, rimelig og effektiv metode for å diagnostisere et bredt spekter av tilstander.

Tolkning og diagnostisering av røntgenbilder innebærer imidlertid en rekke utfordringer. Røntgenbilder inneholder ofte komplekse og overlappende strukturer, noe som kan gjøre det vanskelig å identifisere patologiske forandringer og skille dem fra normale anatomiske varianter. Radiologer må ha høy ekspertise og erfaring for å kunne stille korrekte diagnoser. I tillegg har det økende antallet røntgenbilder som genereres i dagens helsevesen ført til økt arbeidsbelastning for radiologer, noe som kan resultere i tretthet og redusert konsentrasjon, og dermed påvirke nøyaktigheten av diagnostiske vurderinger.

I lys av disse utfordringene har det vokst fram et behov for å utvikle nye metoder og verktøy som kan hjelpe radiologer i deres arbeid med å tolke røntgenbilder og stille nøyaktige diagnoser. Med fremveksten av kunstig intelligens og deep learning har det blitt mulig å utvikle modeller som kan oppnå en høy grad av nøyaktighet og effektivitet i diagnostisering av medisinske tilstander ved hjelp av røntgenbilder. Dette har gitt opphav til et voksende forskningsfelt som fokuserer på å automatisere og forbedre prosessen med å tolke røntgenbilder, og dermed øke diagnostisk nøyaktighet og effektivitet.

Forskning på deep learning og medisinsk bildeanalyse har vist betydelige fremskritt de siste årene, noe som indikerer potensialet for slike teknikker å bli implementert i klinisk praksis. Ved å utvikle en modell som kan identifisere og differensiere mellom ulike diagnoser basert på røntgenbilder, kan dette prosjektet potensielt bidra til å redusere arbeidsbelastningen for radiologer og øke nøyaktigheten av diagnostiske vurderinger. Dette vil igjen kunne føre til bedre behandlingsresultater for pasientene og reduserte kostnader for helsevesenet.

## Data

Fra oppgaven som ble gitt, så fikk vi tilgang til endel data. Dette er de linkene som ble brukt i prosjektet. 

https://stanfordmlgroup.github.io/competitions/chexpert
https://physionet.org/content/mimic-cxr-jpg/2.0.0/
https://cloud.google.com/healthcare-api/docs/resources/public-datasets/nih-chest
https://github.com/ieee8023/covid-chestxray-dataset
https://data.mendeley.com/datasets/jctsfj2sfn/1


## Fremgangsmetode

Prosjektet ble gjennomført av tre personer som samarbeidet for å utvikle en modell for å gjenkjenne brystsykdommer i røntgenbilder. Vi delte oss i tre forskjellige retninger for å utnytte våre ferdigheter og ressurser best mulig. En person var ansvarlig for å samle inn og forberede datasettet, en annen person var ansvarlig for å trene modellen og evaluere resultatene, mens den tredje personen var ansvarlig for å utvikle og implementere Gradio-appen.

For å samle inn og forberede datasettet, brukte vi NIH Chest X-Ray Dataset som er tilgjengelig på Google Cloud Healthcare API. Vi gjorde en grundig undersøkelse av datasettet og tok hensyn til forskjellige faktorer som alder, kjønn og sykdomstyper for å velge ut de mest relevante røntgenbildene. Vi utførte også en grundig datarengjøring og -forberedelse for å sikre at datasettet var egnet for maskinlæring.

Den andre personen var ansvarlig for å trene modellen og evaluere resultatene. Vi brukte et konvolusjonelt nevralt nettverk (CNN) for å bygge modellen og trente den på datasettet. Vi brukte også ulike metrikker som nøyaktighet, F1-score og ROC-kurve for å evaluere modellens ytelse.

Den tredje personen var ansvarlig for å utvikle og implementere Gradio-appen. Gradio er en rask og enkel måte å bygge og distribuere maskinlæringsapplikasjoner på. Appen lar brukerne laste opp et bilde og få en prediksjon av hvilken sykdom som er tilstede, eller om bildet er normalt.

Selv om vi hadde et godt samarbeid og brukte våre ferdigheter og ressurser best mulig, møtte vi noen utfordringer underveis. To av retningene viste seg å ikke være helt vellykket, spesielt når det gjaldt nøyaktigheten til modellen. Vi måtte tilpasse og justere modellen flere ganger for å oppnå ønsket nøyaktighetsnivå. Det var også noen tekniske problemer med implementeringen av Gradio-appen, men disse ble løst ved å kontakte Gradio-support.

Til tross for utfordringene, var det en lærerik opplevelse å jobbe med et reelt dataproblem og å utforske mulighetene og begrensningene ved bruk av maskinlæring i medisinsk diagnostikk. Vi lærte mye om datarengjøring og -forberedelse, modelltuning og evaluering, og utvikling av maskinlæringsapplikasjoner.



## Resultat
Denne rapporten presenterer resultatene av et prosjekt som brukte bryst røntgenbilder fra National Institutes of Health (NIH) Chest X-Ray Dataset. Datasettet inneholder mer enn 100 000 røntgenbilder og er tilgjengelig på Google Cloud Healthcare API. Prosjektet var ment å utforske muligheten for å bruke maskinlæringsteknikker til å lage en modell som kan automatisk gjenkjenne forskjellige brystsykdommer i røntgenbilder.

Etter å ha trent modellen på datasettet og evaluert den ved hjelp av flere metrikker, ble resultatet implementert som en Gradio-app. Gradio-appen lar brukere laste opp et bryst røntgenbilde og få en prediksjon av hvilken sykdom som er tilstede, eller om bildet er normalt. Dessverre viste evalueringen av modellen at den hadde en høy feilrate, spesielt når den skulle skille mellom lungebetennelse og normalt bilde. Dette viser at det er utfordrende å bygge en nøyaktig modell for brystsykdommer på grunn av kompleksiteten i bildene og variasjonen i sykdommene. Det er behov for videre forskning og utvikling for å forbedre nøyaktigheten til modellen.



## Forbedringspotensiale og utbytte av prosjektet
Selv om modellen ikke oppnådde ønsket nøyaktighetsnivå, viser dette prosjektet et stort potensial for anvendelse av maskinlæring i diagnostisering av brystsykdommer. Med tilgang til store og varierte datasett som NIH Chest X-Ray Dataset, kan maskinlæring bidra til å forbedre kvaliteten på diagnose og behandling av pasienter. Videre kan utvikling av mer avanserte modeller og anvendelse av ny teknologi som dyp læring, øke nøyaktigheten og presisjonen til modellene.

Prosjektet kan også bidra til å øke bevisstheten om brystsykdommer og viktigheten av tidlig diagnose. Ved å utvikle en modell som kan gi en rask og nøyaktig diagnose, kan pasienter få raskere tilgang til behandling og bedre prognoser. I tillegg kan dette prosjektet åpne for videre samarbeid mellom medisinske og teknologiske fagområder for å løse komplekse helseproblemer.

Sammenfattende viser dette prosjektet både utfordringer og muligheter for bruk av maskinlæring i diagnostisering av brystsykdommer. Selv om nøyaktigheten til modellen i denne studien ikke var optimal, kan videre forskning og utvikling bidra til å forbedre nøyaktigheten og presisjonen til modellene. Videre samarbeid mellom medisinske og teknologiske fagområder kan også bidra til å utvikle innovative løsninger for å forbedre diagnostiseringen og behandlingen av brystsykdommer.


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
