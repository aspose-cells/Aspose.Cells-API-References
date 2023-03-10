---
title: ErrorCheckOption sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 520
url: /tr/python-net/aspose.cells/errorcheckoption/
is_root: false
---
##  ErrorCheckOption sınıfı
Belirli aralıklarda uygulanan hata kontrolü ayarı.



ErrorCheckOption türü aşağıdaki üyeleri gösterir:

###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [is_error_check(error_check_type)](/cells/tr/python-net/aspose.cells/errorcheckoption/is_error_check/#ErrorCheckType) | Verilen hata tipinin kontrol edilip edilmeyeceğini kontrol eder.|
| [set_error_check(error_check_type, is_check)](/cells/tr/python-net/aspose.cells/errorcheckoption/set_error_check/#ErrorCheckType-bool) | Verilen hata tipinin kontrol edilip edilmeyeceğini ayarlar.|
| [get_count_of_range()](/cells/tr/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | Bu ayardan etkilenen aralıkların sayısını alır.|
| [add_range(ca)](/cells/tr/python-net/aspose.cells/errorcheckoption/add_range/#CellArea) | Bu ayarla etkilenen bir aralık ekler.|
| [get_range(index)](/cells/tr/python-net/aspose.cells/errorcheckoption/get_range/#int) | Verilen dizine göre bu ayarın etkilenen aralığını alır.|
| [remove_range(index)](/cells/tr/python-net/aspose.cells/errorcheckoption/remove_range/#int) | Verilen dizine göre bir aralığı kaldırır.|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells](..)
