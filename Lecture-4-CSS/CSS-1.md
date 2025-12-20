
# CSS 1

Danes bomo spoznali CSS – jezik za oblikovanje videza spletnih strani.

## Kaj je CSS?

CSS (Cascading Style Sheets) je jezik, ki določa, kako naj izgleda HTML dokument. Z njim oblikujemo barve, pisave, razporeditev in druge vidike strani. En CSS lahko upravlja več strani hkrati.

## Sintaksa CSS

CSS pravila so sestavljena iz selektorja in deklaracijskega bloka:

- Selektor določa, kateri HTML elementi bodo oblikovani. Primer: `h1` - selektor za vse naslove prve stopnje.
- Deklaracijski blok vsebuje eno ali več deklaracij, ki določajo lastnosti in njihove vrednosti. Primer: `{ color: blue; font-size: 12px; }`

## CSS Selektorji

Selektorji izberejo elemente, ki jih želimo oblikovati. Nekateri pogosti selektorji so:

- Po elementu: `p`
- Po ID-ju: `#para1`
- Po razredu: `.center`
- Za vse elemente: `*`
- Lahko združimo več selektorjev: `h1, h2, p`

## Kako vnesti CSS v HTML?

CSS lahko vnesemo v HTML na tri načine:

1. Zunanja CSS datoteka: Povežemo CSS datoteko z HTML z uporabo `<link>` v `<head>`.

   ```html
   <link rel="stylesheet" href="datoteka.css">
   ```

2. Notranji slog: Vstavimo CSS znotraj `<style>` v `<head>`.

   ```html
   <style>
     body {
       background-color: lightblue;
     }
   </style>
   ```

3. V določenem elementu: Uporabimo atribut `style` znotraj HTML elementa.

   ```html
   <h1 style="color: blue;">Naslov</h1>
   ```

## Barve v CSS

Barve lahhko določimo na več načinov:

- Z imenom (npr. "Tomato")
- Z RGB
- Z HEX
- Z HSL

Lahko obarvamo ozadje, besedilo, obrobe in druge elemente.

## Oblikovanje besedila

Z CSS lahko spreminjamo videz besedila:

- Spreminjamo barvo
- Spreminjamo postavitev na strani
- Določamo okrasitev (nadčrta, podčrta)
- Definiramo razmik med črkami in vrsticami

## Rob in polnilo

Rob (margin) določa zunanji prostor okoli elementa, medtem ko polnilo (padding) določa notranji prostor znotraj elementa.

Tukaj lahko vidimo, kako to izgleda na sliki.

Od zunanjega proti notranjosti imamo: margin, border (obroba), padding in vsebino (content).

To pomaga razumeti, kako se prostor razporedi okoli elementov.

## Pozicioniranje elementov

Elemente lahko pozicioniramo na različne načine:

- Static: privzeta vrednost, elementi so postavljeni v normalnem toku strani.
- Relative: element je postavljen glede na svojo privzeto pozicijo.
- Absolute: element je postavljen glede na najbližji pozicionirani prednik.
- Fixed: element je postavljen glede na okno brskalnika in ostane na mestu pri pomikanju strani.
- Sticky: element se obnaša kot relative do določenega položaja in nato kot fixed.

## CSS Ikone

Ikone so dodaten nabor znakov/sličic, ki jih lahko uporabimo na spletnih straneh. Pogosto uporabljamo knjižnice ikon, kot je  Google Material Icons.

## Oblikovanje povezav

Povezave (`<a>` elementi) imajo privzete stile, ki jih lahko prilagodimo z CSS:

- `a:link` - stil za neobiskane povezave
- `a:visited` - stil za obiskane povezave
- `a:hover` - stil, ko je kazalec nad povezavo
- `a:active` - stil za aktivno povezavo (ko je kliknjena)

Za vsako stanje lahko določimo različne barve, dekoracije in druge lastnosti.
