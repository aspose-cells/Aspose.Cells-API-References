---
title: get_precedents_in_calculation yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 190
url: /tr/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Hesaplarken bu hücrenin formülü tarafından kullanılan tüm emsalleri (mevcut çalışma kitabındaki hücrelere referans) alır.


###  İadeler

Tüm referansları numaralandırmak için numaralandırıcı(ReferredArea)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Notlar

Bu yöntem yalnızca [FormulaSettings.enable_calculation_chain](/cells/tr/python-net/aspose.cells/formulasettings#enable_calculation_chain)'in geçerli olduğu durumla çalışabilir.
çalışma kitabı için doğrudur ve çalışma kitabı tam olarak hesaplanmıştır.
Bu hücre bir formül değilse veya başka hücrelere referans vermiyorsa, null döndürülür.
###  Örnek

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("A2").get_precedents_in_calculation()
print("A2's calculation precedents:")
for r in en:
    print(r)

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
