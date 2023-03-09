---
title: is_gather_string metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Kontrollerar om det aktuella strängvärdet för cellen måste samlas in i en global pool.


###  Returnerar

true om strängvärdet måste samlas in i en global pool för den resulterande filen.


```python
def is_gather_string(self):
    ...
```


###  Anmärkningar

Att samla in strängvärden kommer bara att dra fördel när det finns många dubblerade strängvärden för cellerna som tillhandahålls av denna implementering.
I denna situation kommer insamlingssträng att spara mycket minne och generera mindre resulterande fil.
Om det finns många strängvärden för cellerna som tillhandahålls av LightCellsDataProvider men få av dem är desamma,
samla sträng kommer att kosta mer minne och tid och har ingen fördel för den resulterande filen.


###  Se även
* modul [aspose.cells](../../)
* klass [LightCellsDataProvider](/cells/sv/python-net/aspose.cells/lightcellsdataprovider)
