---
title: get_dependents_in_calculation yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 100
url: /tr/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır.


###  İadeler

Tüm bağımlıları numaralandırmak için numaralandırıcı(Cell nesneler)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| recursive | bool | Doğrudan bu hücreye başvurmayan bağımlıları döndürür.<br/> ancak bu hücrenin diğer yapraklarına referans|
###  Notlar

Bu yöntemi kullanmak için lütfen çalışma kitabının şu değer için doğru değere ayarlandığından emin olun:
[FormulaSettings.enable_calculation_chain](/cells/tr/python-net/aspose.cells/formulasettings#enable_calculation_chain) ve tamamen bu ayarla hesaplanmıştır.
Bu hücreye herhangi bir formül başvurusu yoksa, null döndürülür.
###  örnekler

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
    print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
    print(c.name)

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
