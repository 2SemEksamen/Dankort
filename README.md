
# Dankort
## Om projektet

Dette projekt er lavet som en del af 2. semesters eksamen. Vi har udviklet et responsivt underwebsite for Dankort Øremærket i Astro med HTML, CSS og JavaScript.

Sitet består af flere sider, hvor brugeren kan:

- læse om Dankort Øremærket  
- se forskellige brugerfordele  
- få information om støtte til naturen  
- navigere mellem forskellige sider og sektioner  

Projektet er bygget med komponenter og responsive layouts, så hjemmesiden fungerer på både mobil, tablet og desktop.

## Links
- GitHub repository:https://github.com/2SemEksamen/Dankort
- Netlify Pages: kommer
- Figma: (https://www.figma.com/design/x24YUmL8RRwHvvjkJx2PVK/Dankort?node-id=1657-2438&p=f&t=vQBrH1IluZ0uIXMl-0)

## Projektstruktur
Projektet er opdelt i astrofiler som indeholder, HTML, Javesqript og css.

```
/
├── public/
│   ├── images/
│   │   ├── app-store.png
│   │   ├── app.webp
│   │   ├── appstoreknap.webp
│   │   ├── dankortgren.webp
│   │   ├── DankortLogo.png
│   │   ├── enlillehandling.webp
│   │   ├── flag.png
│   │   ├── gladevennersammen.webp
│   │   ├── google-play.png
│   │   ├── googleplayapp.webp
│   │   ├── gren.png
│   │   ├── hands.png
│   │   ├── Hjerte.png
│   │   ├── lås.png
│   │   ├── money-cup.png
│   │   ├── stork.png
│   │   ├── telefon-højre.png
│   │   ├── telefon-venstre.png
│   │   ├── tree.png
│   │   ├── træ.png
│   │   └── Velkommen-iphonebilleder.webp
│   ├── favicon.ico
│   └── favicon.svg
│
├── src/
│   ├── assets/
│   │   ├── astro.svg
│   │   └── background.svg
│   │
│   ├── components/
│   │   ├── AppPromo.astro
│   │   ├── BrugerFordele.astro
│   │   ├── BrugerForside.astro
│   │   ├── BytPoint.astro
│   │   ├── DinStotteCard.astro
│   │   ├── FirstScroll.astro
│   │   ├── Footer.astro
│   │   ├── FordeleTekst.astro
│   │   ├── FordeleTekstLI.astro
│   │   ├── FordelsGrid.astro
│   │   ├── FordelsKort.astro
│   │   ├── ForskelInfoCard.astro
│   │   ├── GuestFordele.astro
│   │   ├── GuestForside.astro
│   │   ├── Hero.astro
│   │   ├── HjerteCard.astro
│   │   ├── ImageTextSection.astro
│   │   ├── KontaktBank.astro
│   │   ├── LIRedCTA.astro
│   │   ├── LIVelkommen.astro
│   │   ├── LocalSupport.astro
│   │   ├── LoginSite.astro
│   │   ├── LUVelkommen.astro
│   │   ├── MiniNavbar.astro
│   │   ├── Navbar.astro
│   │   ├── OmOre.astro
│   │   └── RedCTA.astro
│   │
│   ├── layouts/
│   │   └── Layout.astro
│   │
│   ├── lib/
│   │
│   ├── pages/
│   │   ├── fordele.astro
│   │   ├── index.astro
│   │   ├── oere.astro
│   │   └── velkommen.astro
│   │
│   └── types.d.ts
│
├── .gitignore
├── astro.config.mjs
├── package-lock.json
├── package.json
├── README.md
└── tsconfig.json
```
### Filbeskrivelser

- **index.astro** – forsiden til hjemmesiden hvor brugeren kan logge ind eller fortsætte som gæst
- **fordele.astro** – side der viser forskellige brugerfordele og muligheder i universet med point  
- **oere.astro** – side om Dankort Øremærket og hvordan brugeren støtter naturen gennem betalinger  
- **velkommen.astro** – velkomstside til nye og gamle brugere med introduktion til universet  

- **Layout.astro** – fælles layout som bruges på alle sider til struktur, metadata og styling  
- **Navbar.astro** – navigation/menu øverst på siden  
- **MiniNavbar.astro** – mindre navigation
- **Footer.astro** – footer med support, links og information  
- **Components** – genbrugelige komponenter som styrer indholdet på de forskellige sider  
 
- **BrugerFordele.astro** – viser fordele til en logget ind bruger  
- **GuestFordele.astro** – viser fordele til gæster  
- **BrugerForside.astro** – forside til logget ind bruger  
- **GuestForside.astro** – forside til gæstebruger  
 

---

## Hvordan koden fungerer

Vi har opdelt hjemmesiden i komponenter, så hver sektion har sin egen `.astro` fil.

### index.astro

Bruges på login siden.
Her kan brugeren vælge imellem, om de ønsker at logge ind som gæst, eller om de er bruger og derfor vil logge ind.
Alt afhængigt af, hvad de vælger, vil de blive ført til komponentet til brugere eller til gæster.

---

### fordele.astro

Viser forskellige brugerfordele og tilbud, samt viser antal point.

Her bliver komponenter som:
- FordelsKort  
- FordelsGrid  
  

brugt til at vise indhold til brugeren.


---

### oere.astro

Bruges til siden om Dankort Øremærket.

Her bliver indhold omkring:
- naturstøtte  
- donationer  
- brugerens forskel  

vist gennem komponenter som:
- ForskelInfoCard
- Hero  
- OmOre  

---

### velkommen.astro

Bruges som velkomstside til nye eller gamle brugere.

Her bliver forskellige komponenter samlet dynamisk for at opbygge forsiden med:
- hero section  
- app promotion  
- informationssektioner  
- call-to-actions  

---

**Flow:**

1. Siden loader  
2. Astro samler komponenterne  
3. Styling bliver anvendt  
4. Komponenterne bliver vist på siden  
5. Brugeren kan navigere mellem siderne.  

---

## Navngivning

Vi har navngivet vores filer, variabler og funktioner så de så vidt som muligt er selvforklarende.

### Eksempler på variabler

```javascript
const loginBtn 
const guestBtn
const userType 
```

### Eksempler på funktioner

```javascript
if (userType === "bruger") {
  guest.style.display = "none";
}

else {
  bruger.style.display = "none";
}
```

Vi har brugt camelCase i JavaScript, fordi det gør koden mere ensartet og lettere at læse.

---

## Kommentarer i koden

Vi har denne gang ikke gjort brug af kommentarer i koden. Dog kunne det implimenteres senere hen for at kunne hjælpe med forståesen af sammenhæng.


---
## Data og JSON-struktur

Vi henter data fra superbase, som vi selv har lavet.


### Felter vi bruger
- **Id** – bruges til at sende brugeren videre til detaljesiden  
- **Front-title** – titlen der vises på forsiden af kortet  
- **Points** – hvor mange point tilbuddet koster  
- **H2** – overskrift på detaljesiden  
- **Info** – beskrivelse/information om tilbuddet  
- **DateInfo** – dato eller udløbsdato for tilbuddet  
- **Image** – billede til tilbuddet  
- **Kategori** – kategorien tilbuddet tilhører (fx Konkurrencer, Mad & Café, Mode & Sport)  
---



## Git og branches

Vi har brugt GitHub til at samarbejde om projektet.

Vi har arbejdet med branches, så vi ikke sad og ændrede i det samme på samme tid.

Vi navngav branchene med feature først.

### Eksempler på branches

- `hover-fordele`
- `cards-grid`
- `navbar-maya`


### Workflow

1. Lave en branch med navn.
2. Kode en feature
3. Committe ændringer
4. Pushe til GitHub
5. Merge til main når det virkede

Det gjorde det nemmere at holde styr på, hvad der blev lavet og at man kunne gå tilbage i tidligere versioner. 

---

## Bæredygtighed

Vi har tænkt bæredygtighed ind i projektet ved at gøre brug af astro, på den måde har vi kunne holde os til få pages og istedet genbruge komponenter..

**Tiltag:**

- Ingen videoer
- Brug af komponenter



---

## Udfordringer undervejs

En af vores udfordringer var at stylingen fra layout gik tabt på nogle komponenter. I Layour definerede vi skrift størrelser/tykkelser/type samt farve.


**Løsninger:**

- Løsningen her blev at gå ind manuelt og style de komponenter som ikke tog imod stylingen fra Layout. En anden løsning(hvis vi havde haft yderligere tid) kunne have været at oprette en css fil globalt, som kunne hentes hos de forskellige komponenter. 

---

## Mulige forbedringer

Hvis vi skulle arbejde videre med projektet, kunne vi forbedre det ved at tilføje:

- Søgefunktion

---

## Gruppemedlemmer

- Signe Skriver Lorentzen
- Cecilie Due Gregart
- Louise Rasmussen
- Maya Christine Jensen

