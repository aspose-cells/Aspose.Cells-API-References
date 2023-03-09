---
title: AbstractCalculationMonitor klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor klass
Övervaka för användaren för att spåra framstegen i formelberäkningen.



Typen AbstractCalculationMonitor avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [original_value](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Hämtar det gamla värdet för den beräknade cellen.<br/> Bör endast användas i [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) och [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Om cellens värde har ändrats efter beräkningen.<br/> Bör endast användas i [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Hämtar det nyligen beräknade värdet av cellen.<br/> Bör endast användas i [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Implementera denna metod för att göra affärer innan du beräknar en cell.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Implementera denna metod för att göra affärer efter att en cell har beräknats.|
| [on_circular(circular_cells_data)](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Implementera denna metod för att göra affärer när du beräknar formler med cirkulära referenser.|



###  Se även
* modul [aspose.cells](..)
