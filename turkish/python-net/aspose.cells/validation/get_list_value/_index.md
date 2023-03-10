---
title: get_list_value yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Belirtilen hücre için doğrulama listesi için değeri alın.


###  İadeler

Belirtilen hücre için bu doğrulamanın listesini oluşturacak değer.
Liste bir aralığa başvuruyorsa, döndürülen değer bir [ReferredArea](/cells/tr/python-net/aspose.cells/referredarea) nesnesi olacaktır;
Aksi takdirde döndürülen değer boş, nesne[] veya basit nesne olabilir.


```python
def get_list_value(self, row, column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row | int | Satır dizini.|
| column | int | Sütun dizini.|
###  Notlar

Yalnızca türü Liste olan ve verilen hücreye uygulanan doğrulama için,
aksi takdirde null döndürülür.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [ReferredArea](/cells/tr/python-net/aspose.cells/referredarea)
* sınıf [Validation](/cells/tr/python-net/aspose.cells/validation)
