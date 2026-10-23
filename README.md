# Sonde abandonate

Hartă realizată de Ioana Birlan.

Hartă interactivă a inventarului ANRMPSG al sondelor inactive, închise și abandonate (Regulamentul (UE) 2024/1787 privind reducerea emisiilor de metan), pusă lângă penele de metan detectate din satelit, ariile Natura 2000 și obiectivele sensibile din apropiere.

**20,781 sonde** publicate (Etapele I și II), din ~47,135 vizate (44.1%). Pe hartă: 20,745.

Fiecare obiect de pe hartă are sursa în popup: pagina exactă din PDF-ul ANRMPSG, elementul OpenStreetMap, înregistrarea API etc.

## Surse de date

| Sursă | Furnizor | Licență | Stare la generare |
|---|---|---|---|
| [Inventarul sondelor (Reg. UE 2024/1787)](https://www.namr.ro/inventar-sonde-etapa-1-conform-regulament-ue-2024-1787/) | ANRMPSG – Autoritatea Națională de Reglementare în Domeniul Minier, Petrolier și al Stocării Geologice a CO₂ | Informație publică (Legea 544/2001) | ok |
| [Limitele județelor (ADM1)](https://www.geoboundaries.org/) | geoBoundaries – William & Mary geoLab | Creative Commons Attribution 4.0 International (CC BY 4.0) | ok |
| [Pene de metan detectate din satelit](https://data.carbonmapper.org/) | Carbon Mapper (EMIT/NASA, Tanager-1/Planet, AVIRIS-3 etc.) | Termenii de utilizare Carbon Mapper (data.carbonmapper.org) | ok |
| [Surse de emisii din combustibili fosili](https://climatetrace.org/) | Climate TRACE | CC BY 4.0 | ok |
| [Sonde cartate în OpenStreetMap](https://www.openstreetmap.org/copyright) | Contribuitorii OpenStreetMap | ODbL 1.0 | ok |
| [Conducte de petrol și gaze (OSM)](https://www.openstreetmap.org/copyright) | Contribuitorii OpenStreetMap | ODbL 1.0 | ok |
| [Școli, grădinițe, spitale (OSM)](https://www.openstreetmap.org/copyright) | Contribuitorii OpenStreetMap | ODbL 1.0 | ok |
| [Arii protejate Natura 2000](https://www.eea.europa.eu/en/datahub/datahubitem-view/6fc8ad2d-195d-40f4-bdec-576e7d1268e4) | Agenția Europeană de Mediu (EEA) – Natura 2000 (versiunea 2024) | Reutilizare liberă cu atribuire (politica EEA) | ok |
| [Facilități industriale raportoare (E-PRTR)](https://industry.eea.europa.eu/) | Agenția Europeană de Mediu (EEA) – E-PRTR | Reutilizare liberă cu atribuire (politica EEA) | ok |
| [Vânt în timp real](https://open-meteo.com/) | Open-Meteo (modele ICON, GFS, ECMWF etc.) | CC BY 4.0 | ok |
| [Imagini satelitare Sentinel-2 L2A](https://planetarycomputer.microsoft.com/dataset/sentinel-2-l2a) | Copernicus / ESA, prin Microsoft Planetary Computer | Date Copernicus Sentinel, acces liber și gratuit | ok |
| [Hartă de fundal](https://server.arcgisonline.com/ArcGIS/rest/services/Canvas/World_Dark_Gray_Base/MapServer) | Esri World Dark Gray Canvas (Esri, HERE, Garmin, © contribuitorii OpenStreetMap) | Esri – termeni de utilizare, cu atribuire | neîncărcat |
| [Fundal satelitar](https://www.arcgis.com/home/item.html?id=10df2279f9684e4a9f6a7f08febac2a9) | Esri World Imagery (Maxar, Earthstar Geographics) | Esri – termeni de utilizare | neîncărcat |

Generat la 2026-10-23 09:35 UTC cu notebook-ul `harta_sonde_colab.ipynb`.

## Metodologie pe scurt
- Tabelele sunt extrase din PDF prin citirea grilei tabelului (PyMuPDF).
- Coordonatele Stereo70 (EPSG:3844) sunt convertite în WGS84. X/Y inversate au fost detectate la 3,142 sonde, prin verificare cu limita județului declarat.
- Detaliile și limitele sunt în pagina hărții, la „Metodologie și limite”.
