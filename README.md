# The REAL Living Lab

**Reflective Engagement with Analytics for Learning.**

Transformation, witnessed in light. A European-model living lab where citizens, community, public partners and researchers co-create in real-life settings, around one question: does this make someone feel capable?

Director: Dr Etain Kiely · Atlantic Technological University, Galway · ENoLL-aligned, pursuing certification.

## The network

Three teaching sites on one repeatable design, each streaming open environmental data (water, humidity, light, soil):

1. **Gairdín DANÚ** — community site, Annaghdown, Co. Galway
2. **ATU Greenhouse** — academic site, sensor rigs built with Dr Mossy Kelly and his students, ATU Physics Department
3. **Template Greenhouse** — the replicable proving node, built and documented as an open blueprint

## Files in this repository

- `index.html` — the main site (transformation, helix, the work, the network, framework, voices, about)
- `lab-network.html` — the live environmental dashboard for the three sites
- `start-a-site.html` — how to join the network: kit, indicative costs, and a contact form
- `evidence-reels.html` — before/after photo trajectories showing how acts of kindness change a place
- `applied-maths-tadpole.html` — completed applied-maths journal (logistic growth + survival), anonymous, with charts
- `danu.html` — the Gairdín DANÚ page: the place, Voice Beyond Words in full, and the workshops calendar
- `philosophy.html` — the practice of attention (proposed 'our thinking' page)
- `badge-lab.html` — the AI Badge Lab (upload a photo, get a Biodiversity Hero card)
- `biodiversity-heroes.html` — the Hero card collection with the scoring system
- `transformation-tadpole.jpg`, `transformation-froglet.jpg` — the EU GREEN winning image and its sequel
- `enoll-application-backbone.md` — the ENoLL six-block mapping for the self-assessment
- `CNAME` — maps the site to reallivinglab.com
- `README.md` — this file

Upload all files together to the repository.

## Connecting real sensor data

The dashboard (`lab-network.html`) runs on a realistic **simulated feed** out of the box, so the site is alive the moment it deploys. To connect a real site, edit the `SITES` config near the bottom of `lab-network.html` and set that site's `dataUrl` to a JSON endpoint returning:

```json
{
  "site": "danu",
  "timestamp": "2026-06-08T11:40:00Z",
  "water": 58.2,
  "humidity": 64.0,
  "light": 41850,
  "soil": 72.5
}
```

water and humidity in %, light in lux, soil as a 0–100 quality index. A Google Sheet published as JSON, a small static JSON file updated by the rig, or an IoT service (e.g. ThingSpeak) all work. If a feed fails, the site falls back to simulated data gracefully.

## Deploy (GitHub Pages)

1. Create a public repo named `reallivinglab`, upload all files.
2. Settings → Pages → Deploy from a branch → main → / (root) → Save.
3. Point DNS for reallivinglab.com at GitHub Pages (four A records to 185.199.108–111.153, and a www CNAME to your github.io). Add the custom domain in Settings → Pages and enforce HTTPS.

The whole site is static. The Badge Lab's AI scan works inside the Claude artifact preview; to make it work for the public on reallivinglab.com it needs a small serverless proxy holding the API key.

## Principles

Open source. Open data (CC BY-SA 4.0). Privacy by architecture. Co-creation in real-world settings. The love bomb: radical kindness toward self, others and the living world.

## Citation

Kiely, E. (2026). *The REAL Living Lab: Reflective Engagement with Analytics for Learning.* Atlantic Technological University. https://reallivinglab.com

## Contact

Dr Etain Kiely, etain.kiely@atu.ie
