
# HTML 2

Danes se bomo naučili osnove HTML-ja – označevalnega jezika za izdelavo spletnih strani.

## HTML seznami

V HTML lahko ustvarimo tri vrste seznamov:

- Neurejen seznam (naštevanje z oznakami)
- Urejen seznam (oštevilčen)
- Opisni seznam (poimenovanje in opis)

## HTML tabele

Tabele sestavljajo glavni gradniki:

- `<tr>` - vrstica tabele
- `<td>` - podatkovna celica
- `<th>` - celica v glavi tabele

## Colspan

Z atributom colspan lahko celico raztegnemo čez več stolpcev.

Primer: `<td colspan="2">`.

## Rowspan

Z atributom rowspan lahko celico raztegnemo čez več vrstic.

Primer: `<td rowspan="2">`.

## Blokovni elementi

Blokovni elemnti (npr. `<div>`, `<p>`) vedno začnejo novo vrstico in zavzamejo celotno širino.

## Vrstični elementi

Vrstični elementi (npr. `<span>`, `<a>`) ne začnejo nove vrstice in zavzemejo le toliko prostora, kolikor ga potrebujejo,

## HTML ID

ID je enoličen označevalec za posamezen element. Uporablja se za stilizacijo ali dostop v Javascript-u.

## Posebni znaki

Posebne znake (npr. šumnike, simbole) lahko prikažemo s pomočjo kod (npr. `&euro;` za €). Za pravilno kodiranje uporabimo `<meta charset="UTF-8">`.

## Razporeditev

HTML vsebuje posebne elemente za razporeditev vsebine, kot so:

- `<header>` - za glavo strani
- `<nav>` - za navigacijo
- `<footer>` - za nogo strani
- in drugi (`<section>`, `<article>`, `<aside>`)

## Odzivna oblika

Odzivno oblikovanje pomeni, da se spletna stran prilagaja različnim velikostim zaslonov (npr. mobilni telefoni, tablice, računalniki). To dosežemo z uporabo CSS medijskih poizvedb.
