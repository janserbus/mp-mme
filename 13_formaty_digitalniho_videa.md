# 13. Formáty digitálního videa

Video je multimediální kontejner. Obsahuje obraz, zvuk, titulky atd. Pro tvorbu videa je potřeba kokek, který vezme všechna data na vstupu a zformátuje je do příslučného kontejnerů.

## Multimediální kontejner

Multimediální kontejner je typ datového kontejneru, který uchovává různé druhy multimediálních dat (zvuk, obraz, titulky) v jednom souboru.

Tyto kontejnery tedy obsahují různé druhy dat společně s metadaty, které se využívají pro poskitnudí dodatečných informací o obsahu. Například mohou být použity k sinchronizaci audia a videa.

Kontejnery sami o osobě podporují jen určité formáty dílčích dat.

Zbůsob, kterým jsou data v kontejnéru označena a používána, je potřeba standardizovat, čímž vznikly různé formáty těchto kontejnerů.

- __AIFF__ - formát používaný na platformě Mac OS
- __WAV__ - zvukový formát používaný platformou Windows
- __AVI__ - formát pro uchovávání videa a zkuku pro Windows
- __Matroska__- může obsahovat praktický jakýkoliv dílčí formát dat

## Kodek

Kodek je sofrwarový nebo hardwarový nástroj, který kóduje zvuková nebo vizuální data do datového proudu za učelem ukládání, vysílání. nebo streamování. Udělá z analogového vstupu binární výstup, který je možno uložit. Kodeky se poté využívají k opětovnému dekǒdování dat při jejich čtení, čímž se data mohou znovu správně interpretovat.

Data, která kodek vyprodukuje podléhají určitému formátu multimediálního kontejenru.

Muže se jednat o knihovnu nebo program.

Pojem kodek je často zaměňován právě s kodováním na základě něhož pracuje

### Formáty kódování

- H.264 (MPEG-4)
- H.265 (MPEG-H)

### Komprese

Komprese slouží ke snížení objemu dat, při zachování co nejvyšší kavlity.

## Formáty videa

| Název | Přípona souboru | Formát kontejneru | Formát kódování | Formát kódování audia | Použití |
| --- | --- | --- | --- | --- | --- |
| WebM | .webm | Matroska | VP8, VP9 | Vorbis, Opus | Vytvořený pro HTML5 video |
| Matroska | .mkv | Matroska | jakýkoliv | jakýkoliv | Velká podpora jiných formátů |
| AVI | .avi | AVI | jakýkoliv | jakýkoliv | Windows |
| Raw video format | .yuv |  |  |  | Raw video |
| Quick time | .mov | Quick time | několik | MP3 | Apple |
| MP4 | .mp4 | MPEG-4 | H.264, MPEG-4 | MP3, Advanced audio |

## FPS

Počet snímků zobrazených za sekundu. U prokládaného videa se jedná o počet půlsnímků.

## Bitrate

Množství digitálních dat přenesené za jednotku času. Udavá se v bitech za sekundu bit/s.

### Variabilní datový tok

Variace datového toku v závislosti na potřebě

### Konstantní

Po celou dobu bude datový tok konstantní

## Prokládání

Video se dělín na prokládáné (interlanced) a progresivní (progresive).

Prokládané znamená, že během poloviny doby jednoho snímku se nejprve zobrazí liché řádky pixelů a poté v druhé polovině snímku sudé řádky.

Bylo zavedeno pro dosažení lepší kvality s omezenými možnostmi.

Progresivní video zobrazjue snímky najednou.

Prokládané video bylo používáno v minulosti z důvodů ušetření datového toku. V dnešní době se většinou používá progresivní zobrazení.

## PAR / DAR / SAR (Poměr stran pixelu a obrazu)

Různé poměry stran pixelů existují především z historických důvodů, kdy bylo jednodučí tvořit displaje s nečtvercovým poměrem stran pixelu.

Platí rovnice: $DAR = SAR × PAR$

Řekněme že chceme zobrazit obrázek na Full HD dysplaji (1920×1080). Poměr stran 16/9 což odpovídá DAR=1.77.

Pokud bude mít náš obrázek čtvercové pixely tedy PAR=1, tak z předchozí rovnice dostaneme, že SAR=1.77/1 což se rovná 1.77.

Z toho vyplívá, že pokud má obrázek čtvercové pixely DAR a SAR jsou stejné.

Nyní řekněme, že chceme zobrazit obrázek o rozměru 1280×1080, PAR=1.5 na stejný display. Je to možné? SAR = 1280/1080 = 1.185.

Podle vozorečku, když tuto hodnout vynásobíme DAR = SAR * PAR dostaneme zpátky DAR=1.777 což odpovída skutečnému zobrazenému poměru 16/9.

Obrázek má 1280×1080 pixelu, ale poměru stran 1.5 tudíž ve výsledku zabre na displeji stejně místa jako obrázek o rozličení 1920×1080

### Pixel aspect ratio (PAR)

Poměr šířky ku výšce jednotlivých pixelů v digitální fotografii

### Display aspect ratio (DAR)

Poměr šířky ku výšce zobrazeného obrázku neboli poměr skutečných (zobrazených) rozměrů obrázku.

### Storage aspect ratio (SAR)

Poměr šířky ku výšce obrázku v pixelech

## Kombinace různých formátu videi podle fps, řádkování a prokládání

| Druh převodu | Problémy kombinace |
| --- | --- |
| Vše shodné | Bez problému |
| Vyšší fps na nižší | Teoreticky bezproblémové, stačí jen vynechat snímky |
| Nižší fps na vyšší | Musí se vytvořit nové snímky z již existujících, sož je technicky náročné a poskytuje nižší klavlitu a náchilnost k artefaktům |
| Z vyššího rozlišení na nižší | Technicky jednoduche a málo náchilné na chyby |
| Z nižšího rozličení na  vyšší | Technicky náročné, nutá tvorba nových pixelů, vyšší chybovost a náchylnost ke ztrátě dat |
| Progresivní na Prokládané | Technicky náročné, může dojít k zhoršení kvality obrazu a vizuálním artefaktům |
| Prokládané na progresivní | Prokládané video obsahuje poloviční počet snímků, zaroveň je proces technicky nárořný |

## Vytvoři a vyexportovat ukázkové video
