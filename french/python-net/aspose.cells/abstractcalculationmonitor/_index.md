---
title: AbstractCalculationMonitor classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor classe
Surveiller pour que l'utilisateur puisse suivre la progression du calcul de la formule.



Le type AbstractCalculationMonitor expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [original_value](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Obtient l'ancienne valeur de la cellule calculée.<br/> Doit être utilisé uniquement dans [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) et [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [value_changed](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Indique si la valeur de la cellule a été modifiée après le calcul.<br/> Doit être utilisé uniquement dans [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|
| [calculated_value](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Obtient la nouvelle valeur calculée de la cellule.<br/> Doit être utilisé uniquement dans [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate).|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Implémentez cette méthode pour faire des affaires avant de calculer une cellule.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Implémentez cette méthode pour faire des affaires après le calcul d'une cellule.|
| [on_circular(circular_cells_data)](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Implémentez cette méthode pour faire des affaires lors du calcul de formules avec des références circulaires.|



###  Voir également
* module [aspose.cells](..)
