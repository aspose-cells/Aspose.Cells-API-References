---
title: find_formula yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 300
url: /tr/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
Giriş dizesine sahip hücreyi bulur.


###  İadeler

Cell nesne.


```python
def find_formula(self, formula, previous_cell):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| formula | str | Aranacak formül.|
| previous_cell | [Cell](/cells/tr/python-net/aspose.cells/cell) |Aynı formüle sahip önceki hücre. Baştan arama yapılıyorsa bu parametre null olarak ayarlanabilir.|
###  Notlar

Hiçbir hücre bulunamazsa null (Hiçbir şey) döndürür.
 NOT: Bu üye artık kullanılmıyor. Yerine,
lütfen Cells.Find(object,Cell,FindOptions) yöntemini LookInType ile LookInType.OnlyFormulas olarak kullanın
 ve LookAtType, LookAtType.EntireContent olarak.
 Bu üye Kasım 2018 tarihinden itibaren 12 ay sonra çıkarılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
