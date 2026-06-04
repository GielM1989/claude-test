## Dag 5 - Contactformulier (het grote project)

**Wat ik gebouwd heb:**
Een volledig werkend contactformulier met validatie, opslag en berichtenhistorie.

---

**Wat ik geleerd heb:**

**1. Form validatie**
Controleren of iemand correcte data invult voordat je er iets mee doet.
Voorbeeld: naam moet minimaal 2 tekens zijn, e-mail moet een @-teken bevatten.
Zonder validatie kan iemand onzin insturen en gaat je app stuk.

**2. Event listeners**
De pagina luistert naar wat jij doet en reageert daarop.
`addEventListener('input', functie)` = voer deze functie uit na elke toetsaanslag.
Zo werkt real-time feedback — de pagina wacht niet tot je op verzenden klikt.

**3. State management**
De pagina onthoudt dingen: is de knop actief? Is er een melding zichtbaar?
Ik deed dit met een `touched` object dat bijhoudt of je een veld al hebt aangeraakt.
Dit is de basis van hoe React en Vue werken.

**4. localStorage**
Een notitieboekje in je browser dat data onthoudt, ook na het sluiten van de pagina.
`localStorage.setItem('naam', JSON.stringify(data))` = opslaan
`JSON.parse(localStorage.getItem('naam'))` = ophalen
JSON.stringify zet een object om naar tekst (want localStorage slaat alleen tekst op).
JSON.parse doet het omgekeerde: tekst terug naar object.

**5. Dynamische HTML**
Je maakt HTML aan op basis van data, niet met de hand.
Ik had een lijst berichten → de pagina bouwde automatisch een kaartje per bericht.
Meer berichten = meer kaartjes. Minder = minder. De code doet het werk.

---

**Wat moeilijk was:**
- Het verschil tussen `input` en `change` events (dropdown gebruikt change, tekstveld gebruikt input)
- `const` declaraties moeten hoger staan dan waar je ze gebruikt — STORAGE_KEY stond te laag en gaf een fout
- `JSON.stringify` en `JSON.parse` — waarom je niet gewoon een object kunt opslaan

**Wat ik nu snap dat ik eerder niet snapte:**
- Een formulier is niet alleen HTML — de logica eromheen is het echte werk
- localStorage en een database op een server werken hetzelfde principe: opslaan, ophalen, tonen

**Wat ik nog wil leren:**
- Hoe stuur je een formulier écht naar een server (met fetch)?
- Hoe werkt een database op een server vergeleken met localStorage?

---

## Dag 3: Git basics

Wat ik geleerd heb:
- Git is een soort "Apple Time Machine" voor je code
- git init = nieuwe repository starten
- git add = wijzigingen klaarzetten voor opslag
- git commit = wijzigingen definitief opslaan
- git status = welke wijzigingen heb ik open staan?
- git log = geschiedenis van alle commits
- .gitignore = bestanden die Git moet negeren
- git push -u origin main = Bestanden naar Github sturen

Wat moeilijk was:
- Begrijpen waarom je apart "add" en "commit" doet (waarom niet meteen?)

Volgende keer:
- Leer git branch en git checkout




Met Git Push stuur ik het naar Github de online kluis voor alle commmits


## Dag 4 - donderdag
- Vandaag: Git herhaling + site live op Vercel