---
title: set_footer metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells/pagesetup/set_footer/
is_root: false
---
##  set_footer(section, footer_script) {#int-str}
Ställer in ett skript som formaterar sidfoten i en Excel-fil.



```python
def set_footer(self, section, footer_script):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| section | int | 0: Vänster sektion, 1: Mittsektion, 2: Höger sektion.|
| footer_script | str | Skript i sidfotsformat.|
###  Anmärkningar

Skriptkommandon:

| Kommando| Beskrivning|
| :- | :- |
| &P| Aktuellt sidnummer|
| &N| Sidonummer|
| &D| Dagens datum|
| &T| Aktuell tid|
| &A| Bladets namn|
| &F| Filnamn utan sökväg|
| &"<FontName>"| Teckensnittsnamn, till exempel: &"Arial"|
| &"<FontName>, <FontStyle>"| Teckensnittsnamn och teckensnittsstil, till exempel: &"Arial,Fet"|
| &<FontSize>| Teckenstorlek Om detta kommando följs av ett vanligt nummer som ska skrivas ut i rubriken, kommer det att separeras från teckensnittets höjd med ett mellanslag.|
| &K<RRGGBB>|Teckensnittsfärg, till exempel (RÖD): &KFF0000|
| &G| Bildskript|

Till exempel: "&Arial,Fet&8sidfotsanteckning"


###  Se även
* modul [aspose.cells](../../)
* klass [PageSetup](/cells/sv/python-net/aspose.cells/pagesetup)
