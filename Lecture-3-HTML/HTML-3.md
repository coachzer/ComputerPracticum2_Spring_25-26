
# Nadaljujemo z HTML

Danes bomo spoznali, kako z obrazci zbíramo podatke od uporabnikov.

## HTML obrazci

Obrazci so ustvarjeni z `<form>` elementom in vsebujejo različne vnose. Ti podatki se po navadi pošljejo na strežnik za obdelavo ali shranjevanje. Obrazec vedno začenemo in končamo s parno oznako `<form>`.

## Elementi obrazcev

Vnosne podatke zbiramo z elementi `<input>`. Najpogostejši tipi so:

- `<input type="text">` - enovrstični besedilni vnos
- `<input type="radio">` - izbirno polje
- `<input type="checkbox">` - potrditveno polje
- `<input type="submit">` - gumb za pošiljanje obrazca
- `<input type="button">` - navaden gumb za katerkoli namen

## Atributi obrazca

Obrazec ima pomembne atribute:

- `action` - določa, kam se podatki pošljejo ob oddaji obrazca
- `target` - določa, kje se odpre rezultat (npr. `_blank` za novo okno)
- `method` - določa način pošiljanja podatkov (`GET` ali `POST`)
- `autocomplete` - omogoča ali onemogoča samodejno izpolnjevanje obrazca s strani brskalnika
- `novalidate` - onemogoči privzeto preverjanje veljavnosti brskalnika

## Vrste vnosov (`<input type="...">`)

Obstaja veliko vrst vnosnih polj, nekatere vključujejo:

- `password` - za varno vnašanje gesel
- `email` - za vnos e-poštnih naslovov
- `date` - za izbiro datuma
- `number` - za vnos številk
- `file` - za nalaganje datotek
- `color` - za izbiro barve
- `range` - za izbiro vrednosti z drsnikom

## Atributi vnosa

Pomembni atributi za `<input>` so:

- `value` - določa privzeto vrednost vnosa
- `readonly` - naredi vnos samo za branje
- `maxlength` - določa največje število znakov, ki jih je mogoče vnesti
- `min` in `max` - določata minimalno in maksimalno vrednost za številčne vnose
- `multiple` - omogoča izbiro več datotek pri `file` tipu
- `pattern` - določa regularni izraz za validacijo vnosa
- `placeholder` - prikazuje namig v praznem vnosnem polju
- `required` - označuje, da je vnos obvezen
- `step` - določa korak za številčne vnose
