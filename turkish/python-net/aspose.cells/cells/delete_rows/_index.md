---
title: delete_rows yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 260
url: /tr/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Birkaç satırı siler.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row_index | int | Silinecek ilk satır dizini.|
| total_rows | int | Silinecek satır sayısı.|
###  Notlar

Silinen aralık, tablonun (ListObject) üst kısmını (tamamını değil) içeriyorsa,
aralık silinemedi ve hiçbir şey yapılmayacak. MS Excel olarak çalışıyor.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Çalışma sayfasındaki birden çok satırı siler.


###  İadeler




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row_index | int | Satır dizini.|
| total_rows | int | Silinecek satır sayısı.|
| update_reference | bool | Diğer çalışma sayfalarındaki güncelleme başvurularının olup olmadığını gösterir.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
