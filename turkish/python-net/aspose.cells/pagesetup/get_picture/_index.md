---
title: get_picture yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 120
url: /tr/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Üst bilgi / alt bilginin [Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesnesini alır.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesnesini döndürür.
Resim yoksa null döndürür.


```python
def get_picture(self, is_header, section):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| is_header | bool | Üstbilgide mi yoksa altbilgide mi olduğunu gösterir.|
| section | int |0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Üst bilgi / alt bilginin [Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesnesini alır.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesnesini döndürür.


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| is_first | bool | İlk sayfa üst bilgi/alt bilgi resminin alınıp alınmadığını gösterir.|
| is_even | bool | Çift sayfa üst bilgi/alt bilgi resminin alınıp alınmadığını gösterir.|
| is_header | bool |Üstbilgi/altbilgi resminin alınıp alınmadığını gösterir.|
| section | int |0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PageSetup](/cells/tr/python-net/aspose.cells/pagesetup)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
