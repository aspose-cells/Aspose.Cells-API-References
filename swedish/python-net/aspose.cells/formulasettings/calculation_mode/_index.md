---
title: calculation_mode fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode fastighet

Hämtar eller ställer in läget för beräkning av arbetsbok i ms excel.

###  Anmärkningar

Den här egenskapen är endast till för att spara inställningarna i den resulterande kalkylarksfilen
så att andra applikationer (som ms excel) kan agera därefter när de laddar och manipulerar den resulterande filen.
För prestandaövervägande för de flesta användares applikationer, beräknar vi inte någon formel i arbetsboken automatiskt,
oavsett vilket läge som har ställts in för den här egenskapen.
Om användaren behöver beräkna formler, anrop alltid metoder på olika objekt enligt kraven:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/python-net/aspose.cells/cell/calculate), ...etc.
###  Definition:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [CalcModeType](/cells/sv/python-net/aspose.cells/calcmodetype)
* klass [FormulaSettings](/cells/sv/python-net/aspose.cells/formulasettings)
