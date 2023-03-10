---
title: index_of yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 60
url: /tr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Ada göre bir özelliğin dizinini alır.


###  İadeler

Sıfır tabanlı dizin. Bulunmazsa negatif değer.


```python
def index_of(self, name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| name | str | Özelliğin büyük/küçük harf duyarlı olmayan adı.|


##  index_of(item, index) {#DocumentProperty-int}
Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.


###  İadeler

Bulunursa, startIndex'ten son öğeye uzanan dizi listesindeki öğeler aralığındaki değerin ilk oluşumunun sıfır tabanlı dizini; aksi takdirde, -1.


```python
def index_of(self, item, index):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| item | [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) | Dizi listesinde bulunacak nesne. Değer null olabilir.|
| index | int | Aramanın sıfır tabanlı başlangıç dizini. 0 (sıfır) boş bir listede geçerlidir.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.


###  İadeler

dizi listesindeki öğeler aralığındaki değerin ilk geçtiği sıfır tabanlı dizin, startIndex'te başlar ve bulunursa öğe sayısını içerir; aksi takdirde, -1.


```python
def index_of(self, item, index, count):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| item | [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) | Dizi listesinde bulunacak nesne. Değer null olabilir.|
| index | int | Aramanın sıfır tabanlı başlangıç dizini. 0 (sıfır) boş bir listede geçerlidir.|
| count | int | Aranacak bölümdeki öğe sayısı.|



###  Ayrıca bakınız
* modül [aspose.cells.properties](../../)
* sınıf [CustomDocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection)
