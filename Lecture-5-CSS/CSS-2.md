# CSS2

### Slide 1
Za začetek se spomnimo, da je HTML dokument sestavljen iz HTML elementov, ki jih prepoznamo po oznakah oziroma tagih. Zdaj si poglejte slike na slidu in se vprašajte: koliko HTML elementov vidite na njih?

### Slide 2
- Spomnimo se dalje, da je v CSS-ju vsak HTML element obravnavan kot škatla, ne glede na to, ali gre za besedilo, sliko ali kar koli drugega.
- Ta škatla je sestavljena iz štirih delov. Najprej imamo `content`, ki je dejanska vsebina elementa. Okoli vsebine se nahaja `padding`, ki predstavlja notranji odmik med vsebino in robom elementa. Sledi `border` oziroma rob elementa, na zunanji strani pa je `margin`, ki določa razmik med tem elementom in drugimi elementi na strani.

### Slide 3
- CSS vse HTML elemente obravnava na enak način, po t. i. box modelu.
- Ker CSS ne razlikuje med HTML elementi po namenu, lahko skoraj vse CSS ukaze uporabimo za skoraj vse elemente.
- To pomeni, da lahko kateremukoli elementu na enak način spremenimo velikost, dodamo rob, nastavimo notranji in zunanji razmik (padding in margin), background-color ali kar koli drugega.

### Slide 4
Poglejmo si nekaj pogostih CSS lastnosti, ki jih uporabljamo pri oblikovanju seznamov, tabel in slik (W3Schools):

(Seznami)
- Z lastnostjo list-style-type določimo, kakšne oznake ima seznam, na primer pike, številke ali črke.
- Lastnost list-style-image omogoča, da namesto klasičnih pik uporabimo sliko.
- Z list-style-position določimo, ali je oznaka seznama znotraj ali zunaj vsebine elementa.

(Tabele)
- Lastnost border-collapse uporabimo, da tabela izgleda bolj čisto in urejeno; določa, ali se robovi celic združijo v en rob ali ostanejo ločeni.
- Z vertical-align lahko vsebino v celici poravnamo vertikalno, na primer na sredino ali na vrh.

(Slike)
- Lastnost opacity določa prosojnost oziroma neprosojnost elementa.
- Lastnost filter se uporablja za nastavitev vizualnih učinkov slikam (kot so svetlost in zamegljenost, npr. brightness in blur).

### Slide 5
- Strukturo HTML dokumenta si lahko predstavljamo kot drevo.
- Na vrhu drevesa je koren (root), to je celoten HTML dokument, ki se začne z oznako <html>.
- Predniki (ancestors) so vsi elementi, ki se nahajajo nad nekim elementom v strukturi. Na primer: <body> je prednik elementa <p>, če je ta zapisan znotraj <body>.
- Potomci (descendants) so vsi elementi, ki se nahajajo znotraj nekega elementa.
- Starš (parent) je element, ki je neposredno nad nekim elementom.
- Otrok (child) je element, ki je neposredno znotraj drugega elementa.

### Slide 6
- Opiši drevo s svojimi besedami:

# GPT example
<body>

  <section class="main-content">
    <h1>Heading here</h1>
    <p>Lorem ipsum dolor sit amet.</p>
    <p>Lorem ipsum dolor <em>sit</em> amet.</p>
    <hr />
  </section>
  
  <nav class="main-nav">
    <ul>
      <li>item 1</li>
      <li>item 2</li>
      <li>item 3</li>
    </ul>
  </nav>

</body>

Na vrhu tega izseka je element <body>, ki predstavlja koren tega dela dokumenta. Vsi ostali elementi so njegovi potomci.  
Znotraj <body> imamo dva glavna otroka:
- <section class="main-content">
- <nav class="main-nav">

Element <section> je starš elementom <h1>, <p>, <p> in <hr />.  
V drugem odstavku vidimo še element <em>, ki je otrok elementa <p>, hkrati pa potomec elementov <section> in <body>.  
Element <nav> vsebuje seznam <ul>, ta pa ima več elementov <li>. Tukaj lepo vidimo več nivojev drevesa: <nav> → <ul> → <li>.

### Slide 7
- CSS kombinatorji določajo odnose med HTML elementi v drevesni strukturi.
- Ko med dvema selektorjema uporabimo presledek, izberemo vse potomce določenega elementa, ne glede na to, kako globoko v strukturi so (npr. `section p` izbere vse odstavke `<p>` znotraj `<section>`).
- Drugi kombinator je puščica (`>`), ki označuje neposredne otroke.
  (Če uporabimo `nav > ul`, izberemo samo tiste elemente `<ul>`, ki so takoj znotraj elementa `<nav>`.)
- Poleg tega lahko elemente izbiramo tudi bolj natančno, tako da uporabimo razrede ali ID-je (`.moj-razred` izbere vse elemente s tem razredom, `#header-id` izbere element z določenim ID-jem).
- Selektorji atributov: z njimi izberemo elemente glede na njihove atribute (osnovna oblika: tag[attribute]).
- Kasneje bomo še pogledali, kako stilizirati HTML z CSS-om.

### Slide 8
- Zdaj imamo nov pojem: specifičnost oziroma specificity. Specifičnost določa, katero CSS pravilo ima prednost, kadar več pravil vpliva na isti HTML element.
- Zdaj imamo kratko vprašanje: ali kdo ve, kakšne barve bo ta odstavek glede na prikazano kodo na sliki?

### Slide 9
- Bolj specifičen selektor ima večjo prioriteto.
- Selektor, ki velja za vse elemente, ima najnižjo prioriteto. Sledi selektor, ki velja za določen tip elementa (ta ima višjo prioriteto). Nato selektor za elemente z določenim razredom itd. Najvišje v hierarhiji je t. i. inline selektor.

### Slide 10
- Na tem slidu spoznamo meritve v CSS-ju in zakaj so pomembne za prilagodljiv oziroma dinamičen izgled spletnih strani.
- Najprej absolutne meritve: to so fiksne enote, kot so px, cm in mm. Njihova velikost je vedno enaka, ne glede na velikost zaslona ali napravo.
- Absolutne meritve so enostavne za uporabo, vendar niso najbolj primerne za odzivne (responsive) spletne strani.
- Zato uporabljamo relativne meritve, ki omogočajo, da se spletna stran prilagaja različnim velikostim zaslonov, kar je osnova modernega, odzivnega web dizajna.
    - % je odvisen od velikosti starševskega elementa,
    - em je odvisen od velikosti pisave elementa ali njegovega starša,
    - vh predstavlja odstotek višine zaslona,
    - vw predstavlja odstotek širine zaslona.

### Slide 11
- Zdaj si bomo na hitro pogledali nekaj pomembnih CSS lastnosti, ki vplivajo na postavitev in pozicioniranje elementov na spletni strani.
- Lastnost display določa, kako se element prikaže na strani – na primer kot block, inline ali kombinacija obeh. Od tega je odvisno, ali element zavzame celo vrstico in kako se obnaša v odnosu do drugih elementov.
- Z-index uporabljamo, kadar se elementi prekrivajo. Z njim določimo, kateri element je “spredaj” in kateri “zadaj”. Višja vrednost pomeni, da bo element prikazan nad drugimi.
- S CSS-om lahko elemente poravnamo horizontalno, vertikalno ali oboje, odvisno od vrste elementa in načina postavitve.
- Inline-block je poseben način prikaza elementa, ki združuje lastnosti elementov inline in block. Elementi z inline-block se pojavijo v isti vrstici kot drugi inline ali inline-block elementi. Poleg tega lahko za tak element nastavimo lastnosti width, height, margin-top in margin-bottom.
- Na koncu še float. Float se je včasih pogosto uporabljal za postavljanje elementov levo ali desno. Danes se uporablja redkeje, vendar je koristno razumeti, kako deluje, saj ga še vedno najdemo v starejših spletnih straneh.
