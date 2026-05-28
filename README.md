# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).



# Spin_the_recipe
## Om projektet

Dette projekt er lavet som en del af Tema 8. Vi har lavet et dynamisk website med HTML, CSS og JavaScript, hvor indholdet bliver hentet fra et Rest API.

Sitet består af flere sider, hvor brugeren kan:

Se en liste med indhold, klikke sig videre til en detaljeside hvor de kan bruge filtrering, se information om det specifille indhold.

## Links
- GitHub repository:https://github.com/MayaJensen/Spin_the_recipe
- GitHub Pages: https://mayajensen.github.io/Spin_the_recipe/index.html
- Figma: (https://www.figma.com/design/Bx9zIuP7XIadTyRiboYj6D/Spin-the-recipe?node-id=1024-5118&t=bogTyu18cVfwlfIK-0)

## Projektstruktur
Projektet er opdelt i HTML, CSS og JavaScript-filer.
```
project/
├── index.html
├── recipelist.html
├── recipedetails.html
├── css/
│   └── style.css
├── js/
│   ├── index.js
│   ├── recipelist.js
│   ├── recipedetails.js
└── README.md
```

### Filbeskrivelser

- **index.html** – forsiden
- **recipelist.html** – viser en liste med data fra API'et som kan filtreres
- **recipedetails.html** – viser detaljer om en valgt opskrift
- **style.css** – styrer designet
- **JavaScript-filer** – styrer det dynamiske indhold på de forskellige sider

---

## Hvordan koden fungerer

Vi har opdelt JavaScript, så hver side har sin egen js fil.

### index.js

Bruges på forsiden.
Her bliver indhold vist dynamisk, via kategorier hentet fra rest API´et.

### recipelist.js

Henter data fra Rest API'et og viser en liste med opskrifter på siden, som kan filtreres.

**Flow:**

1. Siden loader
2. JavaScript kører
3. Data hentes fra Rest API
4. Data bliver gennemgået med loop
5. HTML bliver indsat i DOM'en
6. Brugeren kan klikke på en opskrift

### recipedetails.js

Bruges til detaljesiden. Den læser et id fra URL'en og henter derefter den rigtige opskrift fra Rest API'et.

Det gør det muligt at genbruge den samme HTML-side til mange opskrifter. I stedet for at lave én side per opskrift, bruger vi ét id i URL'en til at vise det rigtige indhold.


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
- Cecilie Grehart
- Louise Rasmussen
- Maya Christine Jensen

