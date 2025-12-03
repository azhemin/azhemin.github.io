# JSON Harjoitukset - Oppimistehtävät 3a & 3b

Tämä projekti sisältää kaksi erillistä JSON & fetch -harjoitusta.

## Oppimistehtävä 3a - JSON-perusteet

### Tiedostot
- **index.html** - Etusivu, hakee digitekniikat.json-dataa
- **digicafe.html** - Digi Cafe -sivu (ticocafe.json)
- **palaveri.html** - Palaverisivu (palaveri.json)
- **tyot.html** - Vantaan työpaikkailmoitukset
- **ticocafe.json** - Tico Cafe -yrityksen tiedot
- **palaveri.json** - Palaverin tiedot

### Tehtävät
✅ Osa 1: Sivupohja navigointeineen  
✅ Osa 2: Fetch-api ja JSON-käsittely (index.html)  
✅ Osa 3: Oma JSON-data (ticocafe.json & digicafe.html)  
✅ Osa 4: Palaveri-JSON ja -sivu (palaveri.json & palaveri.html)  
✅ Osa 5: Vantaan työpaikat REST-rajapinnasta (tyot.html)

## Oppimistehtävä 3b - Tampere-matka

### Tiedostot
- **tapahtumat.html** - Tampereen tapahtumat Visit Tampere API:sta
- **saa.html** - Helsingin ja Tampereen säätiedot OpenWeatherMap API:sta
- **liikennekamera.html** - Tieliikennekamerakuvat Digitraffic API:sta
- **junat.html** - Junien aikataulut Helsinki-Tampere Digitraffic API:sta

### Tehtävät
✅ Osa 1: Sivupohja navigointeineen  
✅ Osa 2: Tampereen tapahtumat  
✅ Osa 3: Säätiedot Helsingistä ja Tampereelta  
✅ Osa 4: Tieliikennekamerakuvat  
✅ Osa 5: Junien aikataulut

## Käytetyt API:t

### Oppimistehtävä 3a
- Jaakkolan digitekniikat JSON
- Vantaan avoimet työpaikat REST API

### Oppimistehtävä 3b
- **Visit Tampere API** - Tampereen tapahtumat
- **OpenWeatherMap API** - Säätiedot (API Key: `665ecd56dfc08dbb50feb8b8f5034e28`)
- **Digitraffic API** - Liikennekamerat ja junat

## Testaaminen paikallisesti

### Paikallinen web-palvelin (suositeltu)
```powershell
# Python
python -m http.server 8000

# Node.js
npx http-server
```

### VS Code Live Server
Asenna Live Server -laajennus ja avaa sivut sen kautta.

## GitHub Pages -julkaisu

1. Siirrä kaikki tiedostot GitHub-repositorioon
2. Aktivoi GitHub Pages asetuksista (Settings → Pages)
3. Päivitä JSON-tiedostojen URL:t `digicafe.html` ja `palaveri.html` -sivuilla:
   ```javascript
   fetch('https://KÄYTTÄJÄTUNNUS.github.io/ticocafe.json')
   ```

## Huomioita

### Oppimistehtävä 3a
- JSON-validointi: https://jsonformatter.curiousconcept.com/
- Vantaan työpaikka-API voi olla välillä poissa käytöstä

### Oppimistehtävä 3b
- **Säätiedot**: Käytetään opettajan API-avainta
- **Liikennekamerat**: Asema C04507 on esimerkkiasema
- **Junat**: Haetaan pitkän matkan junat jotka pysähtyvät Tampereella (TPE)
- API:t voivat olla välillä hitaita tai poissa käytöstä
