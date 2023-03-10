---
title: register_add_in_function yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 170
url: /tr/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Çalışma kitabına eklenti işlevi ekler


###  İadeler

Eklenti işlevlerini içeren eklenti dosyasının URL'si


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| id | int | Eklenti işlevleri içeren verilerin kimliği,<br/> aynı eklenti dosyası için [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/tr/python-net/aspose.cells/worksheetcollection/register_add_in_function)'in ilk araması ile alınabilir.|
| function_name | str | eklenti işlevi adı|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Çalışma kitabına eklenti işlevi ekler


###  İadeler

Verilen eklenti işlevini içeren verilerin kimliği


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| add_in_file | str | dosya eklenti işlevlerini içerir|
| function_name | str | eklenti işlevi adı|
| lib | bool | verilen eklenti dosyasının Workbook Add-In kitaplığının dizininde mi yoksa alt dizininde mi olduğu.<br/>Bu bayrak, addInFile göreli yol verildiğinde etkili olur ve fark yaratır:<br/> true yolun Eklenti kitaplığına göre olduğunu, false ise yolun bu Çalışma Kitabına göre olduğunu belirtir.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [WorksheetCollection](/cells/tr/python-net/aspose.cells/worksheetcollection)
