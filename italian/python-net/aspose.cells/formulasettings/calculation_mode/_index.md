---
title: calculation_mode proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 60
url: /it/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode proprietà

Ottiene o imposta la modalità per il calcolo della cartella di lavoro in MS Excel.

###  Osservazioni

Questa proprietà serve solo per salvare le impostazioni nel file del foglio di calcolo risultante
in modo che altre applicazioni (come ms excel) possano agire di conseguenza durante il caricamento e la manipolazione del file risultante.
Per considerazioni sulle prestazioni per la maggior parte delle applicazioni dell'utente, non calcoliamo automaticamente alcuna formula nella cartella di lavoro,
indipendentemente dalla modalità impostata per questa proprietà.
Se l'utente deve calcolare formule, chiamare sempre metodi su oggetti diversi in base ai requisiti:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/it/python-net/aspose.cells/cell/calculate), ...ecc.
###  Definizione:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [CalcModeType](/cells/it/python-net/aspose.cells/calcmodetype)
* classe [FormulaSettings](/cells/it/python-net/aspose.cells/formulasettings)
