---
title: create_safe_sheet_name metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 90
url: /sv/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Kontrollerar det angivna arknamnet och skapar ett giltigt vid behov.
Om det angivna arknamnet överensstämmer med reglerna för Excel-arknamn, returnera det.
Annars kommer strängen att trunkeras om längden överskrider gränsen
och ogiltiga tecken kommer att ersättas med ' ', och returnerar sedan det ombyggda strängvärdet.


###  Returnerar




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| name_proposal | str | arknamn som ska användas|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Kontrollerar det angivna arknamnet och skapar ett giltigt vid behov.
Om det angivna arknamnet överensstämmer med reglerna för Excel-arknamn, returnera det.
Annars kommer strängen att trunkeras om längden överskrider gränsen
och ogiltiga tecken kommer att ersättas med ett givet tecken, och returnerar sedan det ombyggda strängvärdet.


###  Returnerar




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| name_proposal | str | arknamn som ska användas|
| replace_char | char | tecken som kommer att användas för att ersätta ogiltiga tecken i det angivna arknamnet|



###  Se även
* modul [aspose.cells](../../)
* klass [CellsHelper](/cells/sv/python-net/aspose.cells/cellshelper)
