# getdailydata – Lakecast

Projecte per obtenir el resum diari de dades Meteocat per a totes les estacions XEMA.

## 🎯 Objectiu

Generar automàticament (cada hora :15 i :45):

- Temperatura màxima del dia
- Temperatura mínima del dia
- Ratxa màxima de vent del dia
- Precipitació acumulada del dia

Els resultats es guarden a:

/data/resum_diari_meteocat.json
/data/resum_diari_meteocat.csv
/data/resum_diari_meteocat.xlsx

Aquest JSON s'utilitza posteriorment per alimentar el banner Lakecast (4 pestanyes).

---

## ⚙️ Execució

El projecte s'executa automàticament mitjançant:

- GitHub Actions (workflow_dispatch)
- Disparat externament per cron-job.org (:15 i :45)

També es pot executar manualment:

```bash
python full_scraper_resum_diari_final.py
# getdailydate
Weather Daily Date Script
