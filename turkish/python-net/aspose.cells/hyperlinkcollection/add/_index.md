---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
Belirli bir hücreye veya bir hücre aralığına köprü ekler.


###  İadeler

[Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink) nesne dizini.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| cell_name | str | Cell adı.|
| total_rows | int | Bu köprü aralığındaki satır sayısı.|
| total_columns | int | Bu köprü aralığının sütun sayısı.|
| address | str | Köprünün adresi.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
Belirli bir hücreye veya bir hücre aralığına köprü ekler.


###  İadeler

[Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink) nesne dizini.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| first_row | int | Köprü aralığının ilk satırı.|
| first_column | int | Köprü aralığının ilk sütunu.|
| total_rows | int | Bu köprü aralığındaki satır sayısı.|
| total_columns | int | Bu köprü aralığının sütun sayısı.|
| address | str | Köprünün adresi.|

###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
Belirli bir hücreye veya bir hücre aralığına köprü ekler.


###  İadeler

[Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink) nesne dizini.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| start_cell_name | str | Aralığın sol üst hücresi.|
| end_cell_name | str | Aralığın sağ alt hücresi.|
| address | str | Köprünün adresi.|
| text_to_display | str | Belirtilen köprü için görüntülenecek metin.|
| screen_tip | str |Belirtilen köprü için ekran İpucu metni.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink)
* sınıf [HyperlinkCollection](/cells/tr/python-net/aspose.cells/hyperlinkcollection)
