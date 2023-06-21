# Senzor CMOS

Obecně jakýkoliv čip musí akumulovat náboj pro daný pixel během expozice, pak převést daný náboj na napětí, zesílit napětí a převést do digitálního formátu

U CMOS senzoru je převod prováděn na jednotlivých buňkách (každá buňka obsahuje potřebný hardware) a poté výsledek pouze přečten po jednotlivých řádcích.

CMOS senzory se dělí na 2 skupiny:

1. __Front-iluminated stucture__ - Elektronika je umístěna před světlocitlivou vrstvou. Což má za nasledek snížení citlivosti.
2. __Back-iluminated structure__ - Elektronika je umístěna za světlocitlivou vrstvou

## CCD senzor (Charge coupled device)

CCD pole umožňuje jednotlivým buňkám předávát akumulovaný náboj okolním buňkám. Toho se využívá při zpracování. Nejprve se jednotliv_ě zpracují pixeli v prvním sloupci a poté jsou všechy ostatní řady převedeny a řadu vedle směrek a začátku a proces se opakuje.

K zpracování všech pixelu je použit jeden převodník.

## Crop factor

Crop factor poměr mezi velikostí diakonály referenčního formátu a velikostídiagonály srovnávanehoformátu daného čipu.

Jako reference se používa kinofilmové políčko (36x24) neboli __fullframe__ senzor.

## Ekvivalentní ohnisková vzdálenost

Ekvivalentní ohnisková vzdálenost je ohnisková vzdálenost přepočítaná na fullfprame senzor.

Pokud mame objektiv určený pro APS-C senzor crop=1.6 při ohniskové vzdálenosti 50mm znamená to, že ekviválentní ohnísková vzdálenost se rovná 50 / 1.6 = 31.25mm

## Parametry senzoru

Vlastnosti CMOS senzoru (v porovnání s CCD senzorem):

- vyšší rychlost zpracování.
- úspornější
- menší citlivost => nižší dynamický rozsah
- levnější výroba

## Bayerova maska

## raw x jpg