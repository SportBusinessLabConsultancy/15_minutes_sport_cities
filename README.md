# 🏟️ 15 Minute Sport Cities

Mappatura e analisi della distribuzione delle strutture sportive nelle principali città europee nell'ottica della città dei 15 minuti, basata su dati OpenStreetMap e distribuzione della popolazione mondiale.

---

## 🗺️ Mappa interattiva

👉 [Visualizza la mappa](https://sportbusinesslabconsultancy.github.io/15_minutes_sport_cities/15%20Minutes%20sport%20cities-mappa%20finale.html)

---

## 📌 Descrizione

Il progetto applica il concetto di "città dei 15 minuti" al dominio sportivo, analizzando in che misura le strutture per il leisure sportivo siano accessibili a piedi o in bicicletta entro 15 minuti dalla residenza nelle principali città europee.

Il modello integra dati sulle strutture sportive estratti da OpenStreetMap tramite Overpass API con dati sulla distribuzione della popolazione (Kontur Population Dataset) per stimare la quota di abitanti con accesso prossimo a infrastrutture sportive e di leisure.

L'analisi copre oltre 30 città europee, producendo una mappa interattiva che consente di esplorare la distribuzione delle strutture sportive, i bacini di accessibilità e la densità di popolazione servita.

---

## 🎯 Obiettivi

- Applicare il framework della città dei 15 minuti al dominio dello sport e del leisure, identificando le aree urbane con buona o scarsa copertura di strutture sportive accessibili a piedi
- Estrarre e processare dati geospaziali sulle strutture sportive (palestre, piscine, campi, parchi sportivi) per oltre 30 città europee tramite OpenStreetMap/Overpass API
- Integrare i dati di distribuzione della popolazione (Kontur H3) con i dati sulle strutture sportive per stimare la quota di residenti con accesso entro 15 minuti
- Sviluppare una mappa interattiva multi-città che consenta confronti tra le diverse realtà urbane

---

## 🔬 Metodologia

Per ciascuna città sono stati estratti tramite Overpass API i dati sulle strutture sportive e di leisure presenti in OpenStreetMap, filtrati per tipologia e qualità del dato. I confini amministrativi sono stati acquisiti separatamente per delimitare l'area di analisi.

La distribuzione della popolazione è stata ricavata dal Kontur Population Dataset, basato su dati H3 a risoluzione standard, e incrociata con i buffer di accessibilità (raggio di 15 minuti a piedi) costruiti attorno a ciascuna struttura sportiva.

L'output finale è una mappa Folium/Leaflet interattiva che visualizza le strutture sportive, le aree di copertura e la densità di popolazione, con possibilità di navigazione tra le diverse città.

---

## 📊 Risultati principali

- Mappate le strutture sportive e di leisure per oltre 30 città europee, con confronto della densità di offerta per abitante
- Stimate le quote di popolazione residente con accesso a strutture sportive entro 15 minuti a piedi
- Identificate le città con maggiore e minore copertura sportiva di prossimità
- Prodotta una mappa interattiva multi-layer per l'esplorazione e il confronto tra città

---

## 🛠️ Tecnologie utilizzate

- **Python / Jupyter Notebook** — elaborazione dati e analisi geospaziale
- **OpenStreetMap / Overpass API** — estrazione dati strutture sportive
- **Kontur Population Dataset** — distribuzione della popolazione mondiale (H3)
- **Folium / Leaflet** — mappa interattiva web
- **GeoPandas** — analisi e manipolazione dati geospaziali

---

## 📁 Struttura del progetto

```
15-Minute-Sport-Cities/
├── README.md
├── 15 MIN CITIES.ipynb
├── 15 Minutes sport cities-mappa finale.html
└── strutture_sportive_dati.xlsx
```

> ⚠️ I dati di input (file GeoJSON per città, dati popolazione) e di output non sono inclusi nel repository per ragioni di dimensione. Le fonti sono indicate nella sezione Dati.

---

## 📂 Dati

| Fonte | Descrizione |
|-------|-------------|
| [OpenStreetMap](https://www.openstreetmap.org) | Strutture sportive e di leisure tramite Overpass API |
| [Kontur Population Dataset](https://data.humdata.org/dataset/kontur-population-dataset) | Distribuzione della popolazione mondiale H3 |

---

## 🔗 Riferimenti

- [What If? - 15 Minute City](https://whatif.sonycsl.it/15mincity/15mincity.php)
- [City Access Map](https://www.cityaccessmap.com)
- [15 Min City AI](https://www.15mincity.ai)

---

## 🔗 Link utili

- 🌐 [Sport Business Lab Consultancy](https://www.sblconsultancy.it/)
