# W3Schools HTML Tutorial

## Elements

- Elementi so osnovni gradniki HTML strani.
- Elementi so predstavljeni z oznakami (tags).
- Elementi imajo lahko atribute, ki določajo dodatne lastnosti.
- Elementi so lahko gnezdeni znotraj drugih elementov.
- Primer elementa: `<p>This is a paragraph.</p>`

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Moj prvi HTML dokument</title>
  </head>
  <body>
    <h1>To je naslov</h1>
    <!-- Dodaj manjši naslov <h2> -->
    <!-- Ovo je komentar -->
    <h2>To je manjši naslov</h2>
    <br>
    <h3>To je še manjši naslov</h3>
    <p>To je odstavek.</p>
  </body>
</html>
```

## Headings

- Kot smo že povedali, naslovi so pomembni za strukturo vsebine.
- Obstaja šest stopenj naslovov, od `<h1>` (najpomembnejši) do `<h6>` (najmanj pomemben).
- Naslovi pomagajo pri organizaciji vsebine.
- Tukaj imamo primer različnih stopenj naslovov:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>This is a Heading 1</h1>
    <h2>This is a Heading 2</h2>
    <h3>This is a Heading 3</h3>
  </body>
</html>
```

## Paragraphs

- Odstavki so osnovni gradniki besedila.
- Odstavki so označeni z oznako `<p>`.
- Odstavki ločujejo besedilo v smiselne enote.
- Primer odstavka:

```html
<!DOCTYPE html>
<html>
  <body>
    <p>To je prvi odstavek.</p>
    <p>To je drugi odstavek.</p>
    <!-- Primer z nenavadnim razmikom med besedami -->
    <p>This    is    a    paragraph    with    extra    spaces.</p>
    <!-- Primer <pre> elementa za ohranjanje oblikovanja -->
    <pre>
This    is    a    paragraph    with    extra    spaces.
This    is    a    paragraph    with    extra    spaces.
This    is    a    paragraph    with    extra    spaces.
This    is    a    paragraph    with    extra    spaces.
    </pre>
    <!-- Primer z uporabo <br> za prelom vrstice -->
    <p>This is a paragraph.<br>This is the second line of the paragraph.</p>
  </body>
</html>
```

## Formatting

- HTML omogoča različne načine oblikovanja besedila.
- Pogosti elementi za oblikovanje vključujejo `<b>`, `<i>`, `<u>`, `<strong>`, `<em>`, in druge.
- Primer oblikovanja besedila:

```html
<!DOCTYPE html>
<html>
  <body>
    <!-- Slovenački: podebljano -->
    <p>This is <b>bold</b> text.</p>
    <!-- Slovenački: ležeče -->
    <p>This is <i>italic</i> text.</p>
    <p>Subscript: H<sub>2</sub>O</p>
    <p>Superscript: E = mc<sup>2</sup></p>
    <p>This is <strong>strong</strong> text.</p>
    <p>This is <em>emphasized</em> text.</p>
    <p>This is <mark>marked</mark> text.</p>
    <p>This is <small>small</small> text.</p>
    <p>This is <del>deleted</del> text.</p>
    <p>This is <ins>inserted</ins> text.</p>
  </body>
</html>
```

## Style Guide

- Pri pisanju HTML kode je pomembno upoštevati določena pravila za boljšo berljivost in vzdrževanje kode.
- Pomembno je, da uporabljamo male začetnice v oznakah in atributih.
- Vedno zapiramo elemente, ki to zahtevajo.
- Primer pravilnega pisanja HTML kode:

```html
<!-- To lahko preskočimo -->
<!DOCTYPE html>
<html>
  <head>
    <title>Proper HTML Example</title>
  </head>
  <body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
  </body>   
</html>
```

## Comments

- To torej lahko preskočimo.
- Komentarji so pomembni za dokumentacijo kode.

## Attributes

- Atributi zagotavljajo dodatne informacije o elementih.
- Atributi so zapisani znotraj začetne oznake elementa.
- Primer atributa:

```html
<!DOCTYPE html>
<html>
  <body>
    <a href="https://www.w3schools.com/">Visit W3Schools</a>
    <a href="https://nsa-splet.si/html/html.php" target="_blank">Visit NSA Splet</a>
    <img src="img_girl.jpg" width="500" height="600">
    <!-- Slika brez atributov širine in višine -->
    <img src="img_girl.jpg"> 
    <!-- Slika z alternativnim besedilom -->
    <img src="img_girlr.jpg" alt="Girl with a jacket">
  </body>
</html>
```

### Style Attributes

- Atributi sloga omogočajo neposredno oblikovanje elementov.
- Primer atributa sloga:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1 style="color:blue;">This is a blue heading</h1>
    <p style="color:red;">This is a red paragraph.</p>
    <p title="I'm a tooltip!">Hover over this paragraph to see the tooltip.</p>
  </body>
</html>

 - `lang` atribut določa jezik strani.
 - SEO (Search Engine Optimization) pomembnost za iskalnike in dostopnost.

- Background Colors

```html
<!DOCTYPE html>
<html>
  <body style="background-color:lightblue;">
    <h1>This page has a light blue background color</h1>
    <p>This is a paragraph.</p>
  </body>
</html>

- Font Family

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="font-family:Arial, sans-serif;">This is Arial font</h1>
        <p style="font-family:'Times New Roman', serif;">This is Times New Roman font.</p>
    </body>
</html>
```

- Font Size

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="font-size:50px;">This is a large heading</h1>
        <p style="font-size:20px;">This is a larger paragraph.</p>
    </body>
</html>

- Text Alignment

```html
<!DOCTYPE html>
<html>
    <body>
        <h1 style="text-align:center;">This heading is centered</h1>
        <p style="text-align:right;">This paragraph is right-aligned.</p>
    </body>
</html>
```

## Colors

- Barve lahko določimo z imeni barv, heksadecimalnimi vrednostmi ali RGB vrednostmi.
- Primer določanja barv:

```html
<!DOCTYPE html>
<html>
  <body>
    <h1 style="color:blue;">This is a blue heading</h1>
    <h1 style="color:#FF5733;">This is a heading with hex color</h1>
    <h1 style="color:rgb(255,0,0);">This is a heading with RGB color</h1>
  </body>
</html>
```

## Images

- Slike se v HTML dodajo z oznako `<img>`.
- Atribut `src` določa pot do slike.
- Atribut `alt` zagotavlja alternativno besedilo za slike.
- Primer vstavljanja slike:

```html
<!DOCTYPE html>
<html>
  <body>
    <h2>Image Example</h2>
    <img src="https://www.w3schools.com/html/img_chania.jpg" alt="Chania" width="600" height="400">
  </body>
</html>
```

## Image Map, Background Image and The Picture Element ????

## File Paths

- Datotečne poti določajo lokacijo datotek na strežniku.
- Obstajajo absolutne in relativne poti.
- Primeri datotečnih poti:

```html
<!DOCTYPE html>
<html>
  <body>
    <h2>Absolute Path Example</h2>
    <!-- Absolutna pot do slike na spletu -->
    <img src="https://www.w3schools.com/html/img_chania.jpg" alt="Chania" width="600" height="400">

    <h2>Relative Path Example</h2>
    <!-- Predpostavimo, da je slika v isti mapi kot HTML datoteka -->
    <img src="images/img_chania.jpg" alt="Chania" width="600" height="400">
  </body>
</html>
```

## Links

- Povezave se ustvarijo z oznako `<a>`.
- Atribut `href` določa ciljno lokacijo povezave.
- Primer ustvarjanja povezave:

```html
<!DOCTYPE html>
<html>
  <body>
    <h2>Link Example</h2>
    <a href="https://www.w3schools.com/">Visit W3Schools</a>
    <!-- Povezava, ki se odpre v novem zavihku -->
    <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools in a new tab</a>
    <!-- Slika kot povezava -->
    <a href="https://www.w3schools.com/">
      <img src="https://www.w3schools.com/images/w3schools_logo_436_2.png" alt="W3Schools Logo" width="100" height="50">
    </a>
    <!-- E-mail povezava -->
    <a href="mailto:someone@example.com">Send Email</a>
    <!-- Gumb kot povezava -->
    <a href="https://www.w3schools.com/">
      <button>Go to W3Schools</button>
    </a>
    <!-- Link Bookmark -->
    <h2 id="section1">Section 1</h2>
    <a href="#section1">Go to Section 1</a>
  </body>
</html>
```

## Lists

- HTML podpira neurejene (unordered) in urejene (ordered) sezname.
- Neurejeni seznami uporabljajo oznako `<ul>`, urejeni pa `<ol>`.
- Posamezni elementi seznama so označeni z oznako `<li>`.
- Primer seznama:

```html
<!DOCTYPE html>
<html>
    <body>
        <h2>Unordered List</h2>
        <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        </ul>
    
        <h2>Ordered List</h2>
        <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
        </ol>

        <h2>Nested List</h2>
        <ul>
        <li>Item 1
            <ul>
            <li>Subitem 1a</li>
            <li>Subitem 1b</li>
            </ul>
        </li>
        <li>Item 2</li>
        </ul>
    </body> 
</html>
```

## Block & Inline

- Blokovni elementi zavzamejo celotno širino razpoložljivega prostora (npr. `<div>`, `<p>`, `<h1>`).
- Vrstični elementi zavzamejo le toliko prostora, kot ga potrebujejo (n
- pr. `<span>`, `<a>`, `<img>`).
- Primer blokovnih in vrstičnih elementov:

```html
<!DOCTYPE html>
<html>
  <body>
    <h2>Block Element Example</h2>
    <div style="background-color:lightgrey;">
      This is a block element (div).
    </div>

    <h2>Inline Element Example</h2>
    <p>This is a paragraph with an <span style="color:red;">inline element (span)</span> inside it.</p>
  </body>
</html>
```
