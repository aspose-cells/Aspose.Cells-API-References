---
title: set_header metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 200
url: /sv/python-net/aspose.cells/pagesetup/set_header/
is_root: false
---
##  set_header(section, header_script) {#int-str}
Ställer in ett skript som formaterar rubriken för en Excel-fil.



```python
def set_header(self, section, header_script):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| section | int | 0: Vänster sektion, 1: Mittsektion, 2: Höger sektion.|
| header_script | str | Skript i rubrikformat.|
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

Till exempel: "&Arial,Fet&8Header Note"


###  Se även
* modul [aspose.cells](../../)
* klass [PageSetup](/cells/sv/python-net/aspose.cells/pagesetup)
