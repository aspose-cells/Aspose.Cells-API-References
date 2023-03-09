---
title: remove_at yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Belirtilen dış bağlantıyı çalışma kitabından kaldırır.



```python
def remove_at(self, index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| index | int | kaldırılacak harici bağlantının dizini.|
###  Notlar

Dış bağlantı kaldırılırken, ona başvuran tüm formüller de kaldırılacaktır çünkü
referanslar geçersiz hale gelir.

##  remove_at(index, update_references_as_local) {#int-bool}
Belirtilen dış bağlantıyı çalışma kitabından kaldırır.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| index | int | kaldırılacak harici bağlantının dizini.|
| update_references_as_local | bool | Verilen harici bağlantının tüm referanslarını geçerli çalışma kitabının referansına güncelleyip güncellemeyeceği.|
###  Notlar

Başvuruların güncellenmesi gerekiyorsa, formüllerdeki dış bağlantılara yapılan başvurular geçerli çalışma kitabına değiştirilecektir.
Örneğin, kaldırılacak harici bağlantı "externalsource.xlam"dır ve "customfunction()" bir özel işlevi tanımlar,
bir hücrenin orijinal formülü "='externalsource.xlam'!customfunction()" şeklindedir,
kaldırdıktan sonra formül "= customfunction()" olacaktır.
Referansların güncellenmesi gerekmiyorsa, bu harici bağlantıya referans veren tüm formüller
bu referanslar geçersiz hale geldiği için de kaldırılacaktır.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [ExternalLinkCollection](/cells/tr/python-net/aspose.cells/externallinkcollection)
