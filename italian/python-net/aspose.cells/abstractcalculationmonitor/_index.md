---
title: classe AbstractCalculationMonitor
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  classe AbstractCalculationMonitor
Monitora per consentire all'utente di monitorare l'avanzamento del calcolo della formula.



Il tipo AbstractCalculationMonitor espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [original_value](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Ottiene il vecchio valore della cella calcolata.<br/> Dovrebbe essere utilizzato solo in [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) e [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Se il valore della cella è stato modificato dopo il calcolo.<br/> Dovrebbe essere utilizzato solo in [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Ottiene il nuovo valore calcolato della cella.<br/> Dovrebbe essere utilizzato solo in [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Implementa questo metodo per fare affari prima di calcolare una cella.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Implementa questo metodo per fare affari dopo che una cella è stata calcolata.|
| [on_circular(circular_cells_data)](/cells/it/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Implementare questo metodo per fare affari quando si calcolano formule con riferimenti circolari.|



###  Guarda anche
* modulo [aspose.cells](..)
