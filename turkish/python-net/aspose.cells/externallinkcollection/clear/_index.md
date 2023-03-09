---
title: clear yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Tüm harici bağlantıları kaldırır.



```python
def clear(self):
    ...
```


###  Notlar

Dış bağlantıları kaldırırken, bunlara atıfta bulunan tüm formüller de kaldırılacaktır çünkü
referanslar geçersiz hale gelir.

##  clear(update_references_as_local) {#bool}
Tüm harici bağlantıları kaldırır.



```python
def clear(self, update_references_as_local):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| update_references_as_local | bool | Dış bağlantıların tüm referanslarını geçerli çalışma kitabının referansları olarak güncelleyip güncellemeyeceği.|
###  Notlar

Başvuruların güncellenmesi gerekiyorsa, formüllerdeki dış bağlantılara yapılan başvurular geçerli çalışma kitabına değiştirilecektir.
Örneğin, bir hücrenin orijinal formülü "='externalsource.xlam'!customfunction()" şeklindedir,
Dış bağlantıları kaldırdıktan sonra, formül "=özelfonksiyon()" olacaktır.
Referansların güncellenmesi gerekmiyorsa, harici bağlantılara referans içeren tüm formüller
bu referanslar geçersiz hale geldiği için de kaldırılacaktır.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [ExternalLinkCollection](/cells/tr/python-net/aspose.cells/externallinkcollection)
