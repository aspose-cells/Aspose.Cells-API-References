---
title: ErrorCheckOption klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 520
url: /sv/python-net/aspose.cells/errorcheckoption/
is_root: false
---
##  ErrorCheckOption klass
Felkontrollinställning tillämpas på vissa intervall.



Typen ErrorCheckOption avslöjar följande medlemmar:

###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [is_error_check(error_check_type)](/cells/sv/python-net/aspose.cells/errorcheckoption/is_error_check/#ErrorCheckType) | Kontrollerar om given feltyp kommer att kontrolleras.|
| [set_error_check(error_check_type, is_check)](/cells/sv/python-net/aspose.cells/errorcheckoption/set_error_check/#ErrorCheckType-bool) | Anger om given feltyp ska kontrolleras.|
| [get_count_of_range()](/cells/sv/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | Hämtar antalet intervall som påverkas av den här inställningen.|
| [add_range(ca)](/cells/sv/python-net/aspose.cells/errorcheckoption/add_range/#CellArea) | Lägger till ett påverkat område av denna inställning.|
| [get_range(index)](/cells/sv/python-net/aspose.cells/errorcheckoption/get_range/#int) | Hämtar det påverkade intervallet för denna inställning av ett givet index.|
| [remove_range(index)](/cells/sv/python-net/aspose.cells/errorcheckoption/remove_range/#int) | Tar bort ett intervall efter givet index.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
