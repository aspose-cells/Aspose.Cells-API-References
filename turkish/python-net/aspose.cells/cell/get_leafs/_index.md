---
title: get_leafs yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 160
url: /tr/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Doğrudan bu hücreye başvuran ve bu hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri alın.


###  İadeler

Tüm bağımlıları numaralandırmak için Numaralandırıcı(Cell)


```python
def get_leafs(self):
    ...
```


###  Notlar

NOT: Bu sınıf artık kullanılmıyor. Yerine,
hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) kullanın.
Bu mülk, Mayıs 2022'den itibaren 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.

##  get_leafs(recursive) {#bool}
Bu hücre değiştirildiğinde güncellenecek olan tüm hücreleri alın.


###  İadeler

Tüm bağımlıları numaralandırmak için Numaralandırıcı(Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| recursive | bool | Doğrudan bu hücreye referans vermeyen yaprakları döndürür.<br/> ancak bu hücrenin diğer yapraklarına referans|
###  Notlar

NOT: Bu sınıf artık kullanılmıyor. Yerine,
hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) kullanın.
Bu mülk, Mayıs 2022'den itibaren 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
