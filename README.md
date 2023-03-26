Chest X-ray
==============================

Prosjektet undersøker deep learning modeller for å utforske x-ray av overkroppen, for å finne avvik fra en frisk kropp. Skal deretter sette riktig diagnose på avvikene


## Introduksjon

Medisinsk bildeanalyse har lenge vært en essensiell komponent i moderne helsetjenester, og
røntgenbilder utgjør en stor del av dette feltet. Radiologer er avhengige av å kunne tolke disse bildene nøyaktig og effektivt for å kunne stille korrekte diagnoser og sikre optimal behandling for pasientene. Imidlertid kan manuell gjennomgang av røntgenbilder være tidkrevende og utsatt for menneskelige feil. I den forbindelse har det vokst fram et behov for å utvikle mer avanserte og automatiserte verktøy som kan bistå radiologer i deres arbeid. Dette prosjektet har som mål å utvikle en deep-learning basert modell som kan identifisere 14 ulike diagnoser gitt en eller flere røntgenbilder.

## Bakgrunn

Røntgenbilder har vært en essensiell komponent innen medisinsk diagnostikk siden oppdagelsen av røntgenstråler av Wilhelm Conrad Röntgen i 1895. Til tross for fremskritt innen andre bildeteknikker som computertomografi (CT), magnetisk resonansavbildning (MRI) og ultralyd, forblir røntgenbilder en rask, rimelig og effektiv metode for å diagnostisere et bredt spekter av tilstander.

Tolkning og diagnostisering av røntgenbilder innebærer imidlertid en rekke utfordringer. Røntgenbilder inneholder ofte komplekse og overlappende strukturer, noe som kan gjøre det vanskelig å identifisere patologiske forandringer og skille dem fra normale anatomiske varianter. Radiologer må ha høy ekspertise og erfaring for å kunne stille korrekte diagnoser. I tillegg har det økende antallet røntgenbilder som genereres i dagens helsevesen ført til økt arbeidsbelastning for radiologer, noe som kan resultere i tretthet og redusert konsentrasjon, og dermed påvirke nøyaktigheten av diagnostiske vurderinger.

I lys av disse utfordringene har det vokst fram et behov for å utvikle nye metoder og verktøy som kan hjelpe radiologer i deres arbeid med å tolke røntgenbilder og stille nøyaktige diagnoser. Med fremveksten av kunstig intelligens og deep learning har det blitt mulig å utvikle modeller som kan oppnå en høy grad av nøyaktighet og effektivitet i diagnostisering av medisinske tilstander ved hjelp av røntgenbilder. Dette har gitt opphav til et voksende forskningsfelt som fokuserer på å automatisere og forbedre prosessen med å tolke røntgenbilder, og dermed øke diagnostisk nøyaktighet og effektivitet.

Forskning på deep learning og medisinsk bildeanalyse har vist betydelige fremskritt de siste årene, noe som indikerer potensialet for slike teknikker å bli implementert i klinisk praksis. Ved å utvikle en modell som kan identifisere og differensiere mellom ulike diagnoser basert på røntgenbilder, kan dette prosjektet potensielt bidra til å redusere arbeidsbelastningen for radiologer og øke nøyaktigheten av diagnostiske vurderinger. Dette vil igjen kunne føre til bedre behandlingsresultater for pasientene og reduserte kostnader for helsevesenet.

[Kaggle -> modell med normal / pneumonia](https://www.kaggle.com/code/evenishell/xrays-chest/edit/run/121576740)




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
