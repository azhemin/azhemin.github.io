# Oppimistehtävä 3 - Palauttamisohjeet

## Tiedostojen sijainti
Kaikki tiedostot ovat kansiossa: `c:\Users\azhem\JSON tehtävät\`

## Palautettavat tiedostot

### Oppimistehtävä 3a (5 HTML + 2 JSON)
1. **index.html** - Etusivu (digitekniikat.json)
2. **digicafe.html** - Digi Cafe
3. **palaveri.html** - Palaveri
4. **tyot.html** - Vantaan työpaikat
5. **ticocafe.json** - Cafe-tiedot
6. **palaveri.json** - Palaveri-tiedot

### Oppimistehtävä 3b (4 HTML)
7. **tapahtumat.html** - Tampereen tapahtumat
8. **saa.html** - Säätiedot
9. **liikennekamera.html** - Liikennekamerat
10. **junat.html** - Junat Helsinki-Tampere

## GitHub Pages -julkaisu

### Vaihe 1: Siirrä tiedostot GitHubiin

Repositoriosi on jo olemassa: **azhemin.github.io**

PowerShellissä navigoi kansioon ja julkaise:

```powershell
cd "c:\Users\azhem\JSON tehtävät"

# Alusta Git (jos ei ole vielä tehty)
git init

# Lisää kaikki tiedostot
git add .

# Tee commit
git commit -m "Oppimistehtävä 3a ja 3b valmis"

# Linkitä GitHub-repositorioon (jos ei ole vielä tehty)
git remote add origin https://github.com/azhemin/azhemin.github.io.git

# Lähetä tiedostot GitHubiin
git branch -M main
git push -u origin main
```

### Vaihe 2: Aktivoi GitHub Pages

1. Mene osoitteeseen: https://github.com/azhemin/azhemin.github.io/settings/pages
2. Source: **Deploy from a branch**
3. Branch: **main** → **/ (root)** → Save

### Vaihe 3: Päivitä JSON-tiedostojen URL:t

Kun GitHub Pages on aktivoitu, päivitä nämä kaksi tiedostoa:

**digicafe.html** - Muuta rivi 43:
```javascript
fetch('https://azhemin.github.io/ticocafe.json')
```

**palaveri.html** - Muuta rivi 47:
```javascript
fetch('https://azhemin.github.io/palaveri.json')
```

Tallenna muutokset ja pushaa uudelleen:
```powershell
git add .
git commit -m "Päivitetty JSON URL:t"
git push
```

### Vaihe 4: Testaa sivustoa

Sivusto on käytettävissä osoitteessa:
- **3a tehtävät:**
  - https://azhemin.github.io/index.html
  - https://azhemin.github.io/digicafe.html
  - https://azhemin.github.io/palaveri.html
  - https://azhemin.github.io/tyot.html

- **3b tehtävät:**
  - https://azhemin.github.io/tapahtumat.html
  - https://azhemin.github.io/saa.html
  - https://azhemin.github.io/liikennekamera.html
  - https://azhemin.github.io/junat.html

## Palautus Moodleen

Jos palautat Moodleen, tee ZIP-paketti:
```powershell
Compress-Archive -Path "c:\Users\azhem\JSON tehtävät\*" -DestinationPath "c:\Users\azhem\Oppimistehtava3.zip"
```

## Tarkistuslista ✓

- [x] Kaikki kommentit poistettu
- [x] Koodi siistiä ja toimivaa
- [x] Fetch API käytössä kaikilla sivuilla
- [x] JSON-tiedon käsittely toteutettu
- [x] For-lauseet taulukoiden läpikäyntiin
- [x] Sisäkkäiset for-lauseet junat.html:ssä
- [x] If-lauseet suodattamiseen
- [x] Responsiivinen tyylittely
- [x] Navigaatio toimii

## Palautettava URL

Palauta opettajalle jompikumpi:
1. **GitHub Pages URL**: https://azhemin.github.io/
2. **ZIP-tiedosto** Moodleen

**DL: 3.12.2025**
