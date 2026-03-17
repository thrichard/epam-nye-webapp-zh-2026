# AI Használati Napló - Webalkalmazás-fejlesztés ZH 2026
**Készítette:** Tóth Richárd
**Használt AI eszköz:** Google Gemini

A ZH során az egyetemi szabályzatnak megfelelően AI asszisztenst használtam a kódolás felgyorsítására és a hibakeresésre. Az alábbiakban összefoglalom a főbb interakciókat és a kapott segítséget.

## 1. JavaScript Logika és Tesztek
**Input/Prompt:** Bemásoltam az `src/js/index.js` tartalmát a két feladathoz (getHighEarners és applyDevBonus), valamint a konzolos teszt kimenetet, amikor az egyik teszt elbukott.

**AI Segítség és Workflow:**
* **Tömbműveletek:** Az AI a `.filter()` és `.map()` beépített JavaScript metódusokat javasolta a megoldáshoz.
* **Hibakeresés (Debugging):** A tesztfuttatás során egy lebegőpontos hiba lépett fel (a `900000 * 1.1` eredménye `990000.0000000001` lett, míg a Vitest pontosan `990000`-et várt). Az AI észrevette a típushibát, és a `Math.round()` alkalmazásával javította a logikát, így az összes teszt (Coverage 100%) zöldre futott le.

## 2. Verziókezelés (Git Workflow)
**Input/Prompt:** Kértem segítséget a fork létrehozásában és a kód beküldésében (Pull Request nyitása).

**AI Segítség:**
* Az AI segített átirányítani a helyi repository origin-jét a saját forkomra (`git remote set-url origin`).
* Lépésről lépésre végigvezetett a megfelelő ágra (branch) történő pusholáson (`git push -u origin tothrichard_FLR7WW`), illetve a GitHub felületén a "Compare & pull request" folyamat helyes elvégzésén.