---
title: ErrorCheckOption classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 520
url: /fr/python-net/aspose.cells/errorcheckoption/
is_root: false
---
##  ErrorCheckOption classe
Paramètre de contrôle d'erreur appliqué sur certaines plages.



Le type ErrorCheckOption expose les membres suivants :

###  Méthodes
| Méthode| Description|
| :- | :- |
| [is_error_check(error_check_type)](/cells/fr/python-net/aspose.cells/errorcheckoption/is_error_check/#ErrorCheckType) | Vérifie si le type d'erreur donné sera vérifié.|
| [set_error_check(error_check_type, is_check)](/cells/fr/python-net/aspose.cells/errorcheckoption/set_error_check/#ErrorCheckType-bool) | Définit si le type d'erreur donné sera vérifié.|
| [get_count_of_range()](/cells/fr/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | Obtient le nombre de plages influencées par ce paramètre.|
| [add_range(ca)](/cells/fr/python-net/aspose.cells/errorcheckoption/add_range/#CellArea) | Ajoute une plage influencée par ce paramètre.|
| [get_range(index)](/cells/fr/python-net/aspose.cells/errorcheckoption/get_range/#int) | Obtient la plage influencée de ce paramètre par un index donné.|
| [remove_range(index)](/cells/fr/python-net/aspose.cells/errorcheckoption/remove_range/#int) | Supprime une plage par index donné.|



###  Exemple

```python
from aspose.cells import CellArea, ErrorCheckType, Workbook

workbook = Workbook()
opts = workbook.worksheets[0].error_check_options
optionIdx = opts.add()
opt = opts[optionIdx]
opt.set_error_check(ErrorCheckType.INCONSIST_FORMULA, False)
opt.set_error_check(ErrorCheckType.INCONSIST_RANGE, False)
opt.set_error_check(ErrorCheckType.TEXT_DATE, False)
opt.set_error_check(ErrorCheckType.TEXT_NUMBER, False)
opt.set_error_check(ErrorCheckType.VALIDATION, False)
opt.add_range(CellArea.create_cell_area("A1", "B10"))
workbook.save(r"Book1.xlsx")

```

###  Voir également
* module [aspose.cells](..)
