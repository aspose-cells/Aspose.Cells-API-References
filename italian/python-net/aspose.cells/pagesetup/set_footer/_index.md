---
title: metodo set_footer
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 180
url: /it/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Imposta uno script che formatta il piè di pagina di un file Excel.



```python
def set_footer(self, section, footer_script):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| section | int | 0: Sezione sinistra, 1: Sezione centrale, 2: Sezione destra.|
| footer_script | str | Script formato piè di pagina.|
###  Osservazioni

Comandi di script:

| Comando| Descrizione|
| :- | :- |
| &P| Numero di pagina corrente|
| &N| Conteggio pagine|
| &D| Data odierna|
| &T| Ora attuale|
| &UN| Nome del foglio|
| &F| Nome file senza percorso|
| &"<FontName>"| Nome del carattere, ad esempio: &"Arial"|
| &"<FontName>, <FontStyle>"| Nome e stile del carattere, ad esempio: &"Arial,Bold"|
| &<FontSize>| Dimensione del font. Se questo comando è seguito da un numero in chiaro da stampare nell'intestazione, sarà separato dall'altezza del carattere con un carattere di spazio.|
| &K<RRGGBB>|Colore del carattere, ad esempio (ROSSO): &KFF0000|
| &G| Sceneggiatura dell'immagine|

Ad esempio: "&Arial,Bold&8Footer Note"


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PageSetup](/cells/it/python-net/aspose.cells/pagesetup)
