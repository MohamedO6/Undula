# Sources, authorship and acknowledgments

## Project

Undula was created by **Team Shiblanga** for NASA Space Apps, **Dancing with the SARs**. The team members are Omar, Mohamed and Islam. This standalone application release is maintained and committed by **Mohamed Tamer** (`MohamedO6`).

The MIT licence and its original copyright notice, **Copyright (c) 2026 Omar Aloush**, are retained in [LICENSE](../LICENSE). A release commit's author identifies that commit and does not replace the project's existing authorship or third-party credits.

## Observation providers

- **NISAR:** NASA/JPL-Caltech and ISRO, accessed through the [Alaska Satellite Facility DAAC](https://search.asf.alaska.edu/) and [NASA Earthdata](https://search.earthdata.nasa.gov/). The [NISAR product guide](https://nisar-docs.asf.alaska.edu/) documents GUNW and GCOV. These bundled products are provisional.
- **Landsat 8/9:** NASA/USGS Collection 2 Level 2 surface reflectance, served through [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/docs/). Scaling and QA follow the [USGS Level-2](https://www.usgs.gov/landsat-missions/landsat-collection-2-level-2-science-products) and [quality-assessment](https://www.usgs.gov/landsat-missions/landsat-collection-2-quality-assessment-bands) documentation.
- **GNSS:** [Nevada Geodetic Laboratory, University of Nevada, Reno](https://geodesy.unr.edu/), with per-station source records in `data/gnss/` and contextual citations in `data/evidence/`.
- **Elevation:** Copernicus DEM GLO-90. © DLR e.V. 2010–2014 and © Airbus Defence and Space GmbH 2014–2018, provided under COPERNICUS by the European Union and ESA.
- **Published context:** The papers and agency reports cited per location remain in `data/evidence/`. They are distinct from measurements computed by this application.

## Maps, images and libraries

- Basemaps and Then & Now: © Esri and imagery partners, including Vantor (Maxar), Airbus and Earthstar Geographics. `data/imagery.json` records dated imagery; source attribution remains in the interface.
- Map context: © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright).
- Ground photographs: the author, licence and source for each photograph are recorded in [data/photos.json](../data/photos.json) and displayed in the application.
- Mapping library: Leaflet 1.9.4, BSD-2-Clause; see [vendor/LEAFLET-LICENSE.txt](../vendor/LEAFLET-LICENSE.txt).
- Evidence timestamps: [OpenTimestamps](https://opentimestamps.org/) and live Bitcoin-chain information. A timestamp supports record integrity, not the validity of a scientific interpretation.
- Typography: Inter and Space Grotesk, delivered through Google Fonts.

Scientific Python dependencies are listed in `pipeline/requirements.txt` and `pipeline/science-requirements.txt`; each dependency retains its own licence.

## AI-assisted elements

Claude through Claude Code and OpenAI Codex assisted development, analysis scripts, review and documentation under team direction and review. Google Flow was used for the astronaut characters. The four Journey illustrations are credited to OpenAI imagegen in [assets/journey/manifest.json](../assets/journey/manifest.json), with file fingerprints.

Illustrations and analytic models are separate from observations. Satellite and GNSS data come from the credited providers; AI tools were not used to fabricate those observations.

## Linked learning resources

The application Guide links NASA remote-sensing/SAR introductions, ARSET training, NISAR StoryMaps, application papers and UAVSAR postcards. Partner links include SAOCOM and RADARSAT catalogues and tutorials. Linked educational or catalogue resources are not additional processed datasets: SAOCOM, RADARSAT and UAVSAR data are not used in the bundled computations.
