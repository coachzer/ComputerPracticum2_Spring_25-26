
# CSS 3

## Slide 1

Danes se bomo ukvarjali s CSS animacijami. Animacije nam omogočajo, da se element **postopoma spreminja** iz enega stila v drug, recimo da se premakne, spremeni barvo, poveča ali zavrti … In to vse brez JavaScript ali katerega koli drugega programskega jezika.

Za animacije najprej potrebujemo **@keyframes** ukaz, ki je v obliki pravila, kjer določimo `potek animacije`, torej kaj se zgodi na začetku, vmes in na koncu. Običajno napišemo `from` in `to` ali pa odstotke, npr. `0%`, `50%`, `100%`, kot bomo videli v naslednjem primeru.

Ko imamo **@keyframes** narejene, animacijo »prilepimo« na element z naslednjimi lastnostmi:

- **animation-name**: tukaj povemo, _katero_ animacijo oz. **@keyframes** naj element uporablja
- **animation-duration**: koliko časa animacija traja, npr. 2 sekundi
- **animation-delay**: koliko časa naj počaka, preden se sploh začne
- **animation-iteration-count**: kolikokrat se animacija ponovi. Lahko je številka ali `infinite`, če želimo, da se vrti neprekinjeno
- **animation-direction**: določi smer predvajanja, na primer `normal` ali `alternate`, kjer gre enkrat naprej, nato nazaj
- **animation-timing-function**: določa tempo animacije – ali je enakomeren ali pa se pospeši oziroma upočasni, npr. `linear`, `ease`, `ease-in`, `ease-out`
- **animation-fill-mode**: določa, kaj se zgodi s stilom _pred_ začetkom ali _po_ koncu animacije, recimo ali element ostane v končnem stanju (`forwards`) ali se vrne na začetek

Zdaj gremo na **prehode (transitions)**. Prehodi omogočajo, da se sprememba stila **ne zgodi takoj**, ampak postopoma. Najpogosteje jih uporabljamo pri interakcijah uporabnika, na primer ko gremo z miško čez gumb ali element (`:hover`).

Osnovna lastnost, ki kontrolira prehode, je **transition**. To je krajša oblika, s katero lahko naenkrat nastavimo več stvari, vendar jih lahko nastavljamo tudi ločeno:

- **transition-property**: določa, _katera lastnost_ naj se animira. To je lahko na primer `background-color`, `width`, `transform` ali pa `all`, če želimo, da se animirajo vse spremembe
- **transition-duration**: pove, kako dolgo traja prehod, na primer 0.3 sekunde ali 1 sekundo
- **transition-delay**: določa zamik, torej koliko časa naj počaka, preden se prehod začne
- **transition-timing-function**: določa potek prehoda, ali je gibanje enakomerno ali pa se pospeši oziroma upočasni, na primer `linear`, `ease`, `ease-in`, `ease-out`

Če vse to združimo, lahko z eno samo vrstico povemo: _katera lastnost se spreminja, kako dolgo traja prehod, kdaj se začne in kako poteka_.

Pomembno je razumeti razliko: **transitions reagirajo na spremembo stila** (na primer `:hover`), medtem ko **animacije tečejo same po sebi**, neodvisno od uporabnikovega dejanja.

Zdaj si poglejmo **CSS transformacije**. Transformacije nam omogočajo, da element **premaknemo, zavrtimo, povečamo, pomanjšamo ali poševno nagnemo**, ne da bi vplivali na razporeditev drugih elementov na strani.

Vse transformacije nastavljamo z lastnostjo **transform**, ki vsebuje eno ali več funkcij hkrati.  
Najpogostejše funkcije so:

- **translate()**: premakne element po osi X in Y. Element se premakne vizualno, vendar ostane na istem mestu v layoutu
- **rotate()**: zavrti element za določen kot, na primer za 45 stopinj
- **scaleX()** in **scaleY()**: povečata ali pomanjšata element samo po eni osi – vodoravno ali navpično
- **scale()**: poveča ali pomanjša element enakomerno po obeh oseh
- **skewX()** in **skewY()**: poševno nagne element po osi X ali Y
- **skew()**: omogoča nagib po obeh oseh hkrati

## Slide 2

Da si boste animacije lažje predstavljali, poglejmo kratek posnetek, ki predstavlja **analogijo s flipbook animacijo**
