<div align="center">
  <h1 align="center">RoundIt</h1>

  <p align="center">
    <a href="https://github.com/connorjonesy/roundit/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/connorjonesy/roundit.svg?style=for-the-badge" alt="Contributors" />
  </a>
  <a href="https://github.com/connorjonesy/roundit/network/members">
    <img src="https://img.shields.io/github/forks/connorjonesy/roundit.svg?style=for-the-badge" alt="Forks" />
  </a>
  <a href="https://github.com/connorjonesy/roundit/stargazers">
    <img src="https://img.shields.io/github/stars/connorjonesy/roundit.svg?style=for-the-badge" alt="Stargazers" />
  </a>
  <a href="https://github.com/connorjonesy/roundit/issues">
    <img src="https://img.shields.io/github/issues/connorjonesy/roundit.svg?style=for-the-badge" alt="Issues" />
  </a>   <br />  <br />
    Have you ever crossed an intersection and felt unsafe? Yeah. Us too. <br />
    <br />
    Welcome to RoundIt <br /> <br />
    Safer intersections start with understanding the data.
    <br />
    Explore reported intersection crashes across British Columbia.
    <br />
    <br />
    This was built for <a href="https://devpost.com/software/roundit"><strong> StormHacks 2026</strong></a>
    <br />
    <br />
    <a href="https://www.roundit.tech/"><strong> It's also deployed! (roundit.tech)</strong></a>
    <br />
    <br />
    <a href="https://github.com/connorjonesy/roundit/issues">Report Bug</a>
    ·
    <a href="https://github.com/connorjonesy/roundit/issues">Request Feature</a>
  </p>
</div>

<div align="center">
  <h3>Built With</h3>

  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/MapLibre_GL_JS-396CB2?style=flat-square&logo=maplibre&logoColor=white" alt="MapLibre GL JS" />
  <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" alt="Three.js" />
  <img src="https://img.shields.io/badge/Vanilla_UI-0891B2?style=flat-square" alt="Vanilla UI" />
  <img src="https://img.shields.io/badge/GeoJSON-438026?style=flat-square" alt="GeoJSON" />

  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/KaggleHub-20BEFF?style=flat-square&logo=kaggle&logoColor=white" alt="KaggleHub" />
</div>

## About The Project

Intersections can sometimes be dangerous and inefficient. [Translink's 2040 Transportation Plan](https://vancouver.ca/files/cov/transportation-2040-plan.pdf) aims to create zero traffic related fatalities, we want to aid in that effort. 

RoundIt explores how more accessible collision data can support conversations
about safer streets. Our longer-term goal is to help identify intersections
worth investigating for redesign, including possible roundabout conversions.

The current application maps reported intersection crashes across British
Columbia. An interactive heatmap highlights relative crash concentration,
while individual intersection markers show reported counts, pedestrian and
cyclist involvement, and the reporting period.

Note: RoundIt currently provides data exploration. Assessing whether an intersection
would benefit from a roundabout requires further analysis, which we plan on adding in the near future. 

### Features

- **Interactive map:** Explore intersections all around BC. 
- **Crash heatmap:** View crash concentration.
- **Intersection details:** Click a marker to see total reported crashes,
  pedestrian-involved crashes, cyclist-involved crashes, and reporting years.
- **Layer controls:** Toggle the heatmap and intersection markers independently.
- **3D roundabout:** Three.js is pretty cool right? :).
- **Responsive layout:** Browse the map on desktop and smaller screens.

## Project Structure

```text
roundit/
├── frontend/
│   ├── index.html                 Sidebar and page markup
│   ├── src/
│   │   ├── main.ts                Application entry point
│   │   ├── mapLibre.ts            Map setup and navigation
│   │   ├── intersectionLayers.ts  Heatmap and intersection layers
│   │   ├── 3d/                    Animated roundabout scene
│   │   ├── styles/                Theme, layout, and component styles
│   │   └── ui/                    Controls and intersection popups
│   ├── scripts/                   CSV-to-GeoJSON export
│   └── public/data/               Generated map data
├── backend/
│   ├── app/                       API and database integration code
│   ├── data/                      Cleaned records and summaries
│   └── ingest/                    Data cleaning and aggregation
└── vercel.json                    Deployment configuration
```

## Acknowledgments

- ICBC crash data, accessed through the Kaggle dataset configured in the
  ingestion script.
- [OpenFreeMap](https://openfreemap.org/) for the map style and tiles used
  by the application.
- [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors.
- The open-source libraries that power the map, interface, and 3D preview.

lorem ipsum. :)

<!-- <p><strong>Backend Integration</strong></p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Uvicorn-4051B5?style=flat-square" alt="Uvicorn" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" /> -->

<!-- ## About The Project

Intersections can sometimes be dangerous and inefficient.

RoundIt explores how more accessible collision data can support conversations
about safer streets. Our longer-term goal is to help identify intersections
worth investigating for redesign, including possible roundabout conversions.

The current application maps reported intersection crashes across British
Columbia. An interactive heatmap highlights relative crash concentration,
while individual intersection markers show reported counts, pedestrian and
cyclist involvement, and the reporting period.

Note: RoundIt currently provides data exploration. Assessing whether an intersection
would benefit from a roundabout requires further analysis, which we plan on adding in the near future. 

### Features

- **Interactive map:** Explore intersections all around BC. 
- **Crash heatmap:** View crash concentration.
- **Intersection details:** Click a marker to see total reported crashes,
  pedestrian-involved crashes, cyclist-involved crashes, and reporting years.
- **Layer controls:** Toggle the heatmap and intersection markers independently.
- **3D roundabout:** Three.js is pretty cool right? :).
- **Responsive layout:** Browse the map on desktop and smaller screens.


# Have you ever crossed an intersection and felt unsafe. Yeah. Us too. 

### Welcome to roundit. We imagine a world in which intersections are removed, and in their place, roundabouts rule the world. Pedestrians can cross safely, cars are forced to slow down, drivers focus more, cyclists remain unscathed. 

[Translink's 2040 Transportation Plan](https://vancouver.ca/files/cov/transportation-2040-plan.pdf) aims to create zero traffic related fatalities, we want to aid in that effort. 

Roundabouts have been proven to significantly reduce intersection collisions around the world. They help keep every type of road user safe. 

Our goal was to identify intersections with high collision rates and help determine which of them could benefit from being redesigned as roundabouts. By making collision data more accessible, we hope to encourage safer and more informed urban planning decisions in Vancouver. 

#### Contributing Notes

### Dev environemnt

* serve the backend with uvicorn: `uvicorn main:app --reload`

* serve the frontend with vite: 

`npm install`

`npm run dev`


/

# requirements-ingest.txt

To Ingest that crap locally, use a virtual environment

```
python3 -m venv .venv-ingest
source .venv-ingest/bin/activate
pip install -r requirements-ingest.txt
```
# How does it work?

We ingest and update our DB in the ingest directory (Follow the respective README)

The frontend will query our web service to retrieve necessary data.

(At the moment, we have pulled in Vancouver data to live in the frontend. But we can remove this at anytime and only rely on the render postgres DB)

lorem ipsum. :)

### PROD

* render backend (postgres db and web service)
* vercel frontend -->


