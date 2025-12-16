# Slide 1

HTML je jezik, v katerem so napisane skoraj vse spletne strani. Kratica pomeni HyperText Markup Language, kar lahko prevedemo kot »jezik za označevanje hiperteksta«. To ni programski jezik v klasičnem smislu, ampak jezik, s katerim je opisana struktura strani – kaj je naslov, kje je slika, povezava, gumbin tako naprej.

HTML je bil razvit leta 1993, in je še danes osnovni standard za pisanje spletnih strani. Vsi sodobni brskalniki razumejo HTML.

Spletna stran napisana v HTML-u je sestavljena iz elementov. Na primer, imamo poseben element za naslov, element za besedilo, element za slike in tako naprej. Vsak element ima svojo posebno oznako (tag), s katero ga zapišemo v kodi. Na naslednjih slajdih bomo videli, kako te oznake izgledajo in kako jih uporabljamo.

# Slide 2

Torej, kot smo rekli elementi brskalniku povejo, kako naj prikaže posamezne dele strani. 

V HTML-u jih zapišemo takole: Torej na začetku napišemo začetno oznako, potem sledi vsebina, ki jo želimo prikazati, in na koncu dodamo še zaključno oznako

Elementi se lahko tudi vstavljajo ene v drugega – temu rečemo gnezdenje- in to nam omogoča gradnjo bolj kompleksnih delov spletne strani.

# Slide 3

Zdaj tukaj imamo en preprost primer.

- <!DOCTYPE html> pove brskalniku, da je dokument napisan v HTMLu 5. To je samo deklaracija in ni del same vsebine strani.

- <html> označujejo korenski element vsake HTML strani – v njem se nahajajo vsi ostali elementi

- <body> predstavlja vidni del spletne strani. Tukaj so vsi naslovi, odstavki, slike, povezave, tabele, seznami in druge vsebine ki jih vproabnik vidi
- <h1> označuje največje zaglavlje oz. heading na strani.
- <h2> je nekoliko manjši heaading oz. heading z manjšo velikostjo besed. Obstajajo pa tudi <h3>, <h4> … vse do <h6>
- <p> označuje odstavek besedila

# Slide 4

HTML elementi lahko vsebujejo atribute. Atributi brskalniku dajo dodatne informacije o elementu, na primer v katerem jeziku je stran, kakšen je naslov slike, kam vodi povezava itd. 
Atribute najpogosteje zapišemo kot par ime–vrednost, na primer na prikazani kodi atribut lang pove, da je stran napisana v angleščini.

# SLide 5

Za pisanje HTML kode lahko uporabljamo različne urejevalnike besedila oz. text editorje.
- Najbolj osnovna sta Notepad na Windows in TextEdit na Macu.
- Na Linuxu imamo več možnosti, na primer Nano, Vim, Gedit ali Sublime Text.
- Lahko uporabljamo tudi bolj komplicirane urejevalnike, kot je Visual Studio Code, ki nam omogoča dodajanje različnih pluginov za lažje pisanje kode.
- Neodvisno od editorja, najbolj pomembna stvar je da datoteko s HTML kodo shranimo shranimo s končnico .html ali .htm in je nato lahko odpremo v katerem koli spletnem brskalniku

# Slide 6

- HTML bonton pomeni nekaj osnovnih pravil, ki jih upoštevamo pri pisanju HTML kode, da je koda pregledna in razumljiva 
- Najprej moramo dokument vedno začeti z ustrezno deklaracijo torej z `<!DOCTYPE html>`
- Pri pisanju HTML elementov vedno uporabljamo male začetnice v oznakah
- Zelo pomembno je tudi, da vse elemente zapremo, ko jih zaključimo.

# SLide 7
- Atribute tudi vedno zapišemo z malimi začetnicami
- Vrednosti atributov morajo biti zapisane v navednicah
- Pomembno je tudi, da okoli enačajev ni presledkov

# Slide 8
- Končno, moramo pri pisanju HTML-ja paziti tudi na pravilno strukturo dokumenta
- To pomeni, da elemente, kot so <body>, <h1>, <h2>, <p> in drugi, postavljamo v pravilnem zaporedju in jih smiselno organiziramo.
- Struktura naj bo logična: najprej naslov, potem podnaslovi, nato odstavki in ostala vsebina.
