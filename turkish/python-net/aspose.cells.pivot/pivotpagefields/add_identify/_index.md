---
title: add_identify yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Veri aralığını tanımlamak için her sayfa alanındaki hangi öğe etiketinin kullanılacağını ayarlar.
pageItemIndex.Length, PageFieldCount'a eşit olmalıdır, bu nedenle lütfen önce sayfa alanını ekleyin.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| range_index | int | Konsolidasyon veri aralığı dizini.|
| page_item_index | list | Her sayfa alanındaki sayfa öğesi dizini.<br/>pageItemIndex[2] = 1, üçüncü alandaki bu aralığı tanımlamak için kullanılacak ikinci öğe anlamına gelir.<br/> pageItemIndex[1] = -1, ikinci alanda bu aralığı tanımlamak için kullanılacak öğe olmadığı anlamına gelir<br/> ve MS, bu aralığı tanımlamak için ikinci alanda otomatik olarak "boş" öğe oluşturacaktır.|



###  Ayrıca bakınız
* modül [aspose.cells.pivot](../../)
* sınıf [PivotPageFields](/cells/tr/python-net/aspose.cells.pivot/pivotpagefields)
