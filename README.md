# CI/CD Labor: Flask API Automaatne Pipeline

Selles projektis õppisin, kuidas seadistada **pidevat integratsiooni ja tarnimist (CI/CD)** GitHub Actions abil, ehitada Docker konteinerit, kirjutada teste ja deploy’ida rakendust turvaliselt.

---

## Projekti eesmärk

Eesmärk oli luua **Flask API**, mis sisaldab:

- `/` - põhiinfo
- `/health` - tervisekontroll
- `/products` - toodete nimekiri
- `/api/version` - versiooniinfo
- `/api/status` - API oleku info  

Ja seadistada selle jaoks **CI/CD pipeline**, mis kontrollib:

1. Python süntaksit (validate stage)  
2. Automaatseid teste (test stage)  
3. Docker build + health check (build stage)  
4. Manual deployment production’i (deploy stage)  

---

## Mida õppisin

### 1. Git ja GitHub

- Kuidas alustada uut projekti ja luua `main` branch  
- Kuidas seadistada remote repository ja push’ida koodi  
- Branchide ja commit’ide haldamine  

### 2. GitHub Actions ja CI/CD

- Pipeline loomine `.github/workflows/ci.yml`  
- **Validate stage** – kiire süntaksi kontroll  
- **Test stage** – pytest abil äriloogika kontroll  
- **Build stage** – Docker image loomine ja health check  
- **Deploy stage** – production deploy koos manual approval’iga  
- Workflow’ logide lugemine ja vigade debugimine  

### 3. Python ja Flask

- REST API loomine Flaskiga  
- JSON response’de koostamine  
- Testide kirjutamine `pytest` abil  
- Testide tähtsus: süntaks ja äriloogika kontroll  

### 4. Docker

- Dockerfile loomine ja konteineri buildimine  
- Kohalikult konteineri jooksutamine ja health check  
- CI/CD build pipeline’i integreerimine Dockeriga  

### 5. Vigade leidmine ja parandamine

- Tahtlike vigade loomine laboris:  
  - Süntaksi viga  
  - Negatiivne hind toodetes  
  - Vale versioon  
  - Vale port Dockerfile’is  
- Kuidas pipeline need vead avastab ja kuidas neid parandada  

---

## Pipeline väärtus

- **Validate** – kiireim viis leida süntaksivead  
- **Test** – kontrollib äriloogikat, mida süntaks ei leia  
- **Build** – tagab, et rakendus töötab konteineris  
- **Deploy** – production vajab manual approval’i kõrge riski tõttu  

---

## Tulevased sammud ja täiustused

- Uute endpoint’ide lisamine ja testimine  
- Multi-environment deployment (dev/staging/prod)  
- CI/CD laiendamine teistesse projektidesse  
- Automaatne rollback vanemale versioonile  

---

## Kokkuvõte

See labor andis mulle praktilise kogemuse:

- CI/CD pipeline loomine ja debugimine  
- Automaatsete testide ja Docker build’i integreerimine  
- Vigade avastamine ja parandamine GitHub Actions abil  
- Koodi turvaline deploy production’i  

🎯 **Ahaa moment:** Mõistsin, et validate ja test kontrollivad täiesti erinevaid asju, ja Docker health check on kriitiline enne production’i deploy’d.  

