# KK1 - Video Game Sales

Det här repot innehåller min notebook för Kunskapskontroll 1 i kursen Artificiell Intelligens - programmering Python.

## Dataset

Jag använder datasetet `vgsales.csv`, som innehåller rapporterad försäljning av tv-spel per region. Datasetet kommer från [Video Game Sales på Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales), som i sin tur bygger på data från VGChartz.

Varje rad verkar representera ett spel på en specifik plattform. Datasetet innehåller bland annat:

- spelnamn
- plattform
- år
- genre
- publisher
- försäljning i Nordamerika
- försäljning i Europa
- försäljning i Japan
- försäljning i övriga regioner
- global försäljning

Försäljningen anges i miljoner exemplar.

Datasetet verkar täcka spel fram till ungefär 2017. Det bör därför inte tolkas som en komplett bild av dagens spelmarknad, särskilt eftersom digital försäljning, mobilspel och nya affärsmodeller troligen inte fångas fullt ut.

## Syfte

Syftet med analysen är att undersöka mönster i global och regional spelförsäljning. Jag fokuserar särskilt på:

- vilka genrer som dominerar global försäljning
- hur försäljningen förändras över tid
- hur regioner skiljer sig i genreprofil
- hur toppspel och outliers påverkar helhetsbilden
- om Nordamerika och Europa verkar ha liknande smakmönster

## Struktur

```text
notebook.ipynb
data/
  vgsales.csv
README.md
requirements.txt
```

## Köra projektet

För att köra notebooken lokalt behövs Python och Jupyter Notebook.

Skapa en virtuell miljö:

```powershell
python -m venv .venv
```

Aktivera miljön i PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Installera paketen:

```powershell
pip install -r requirements.txt
```

Starta Jupyter Notebook:

```powershell
jupyter notebook
```

När Jupyter öppnas i webbläsaren, öppna filen:

```text
notebook.ipynb
```

Notebooken förväntar sig att datasetet ligger här:

```text
data/vgsales.csv
```

## Paket

Analysen använder:

- pandas
- numpy
- matplotlib
- jupyter
- ipykernel

Dessa finns i `requirements.txt`.

## Inlämning

Den färdiga analysen finns i `notebook.ipynb`.