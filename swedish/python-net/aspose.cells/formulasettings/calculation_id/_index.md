---
title: calculation_id fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id fastighet

Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken.

###  Anmärkningar

Den här egenskapen är endast till för att spara inställningarna i den resulterande kalkylarksfilen
så att andra applikationer (som ms excel) kan agera därefter när de laddar och manipulerar den resulterande filen.
I fallet med ms excel, om värdet på den här egenskapen är mindre än den associerade omräkningsmotorns identifierare
med programmet som öppnar den resulterande filen, kommer programmet att räkna om resultaten av alla formler
på den här arbetsboken omedelbart efter att filen laddats.
För prestandaöverväganden för de flesta användares applikationer, beräknar vi inte någon formel i arbetsboken automatiskt,
oavsett vilket värde som har satts för denna fastighet.
###  Definition:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [FormulaSettings](/cells/sv/python-net/aspose.cells/formulasettings)
