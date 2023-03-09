---
title: import_xml yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 220
url: /tr/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Bir XML veri dosyasını çalışma kitabına aktarır/günceller.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| url | str | xml dosyasının url'si/yolu.|
| sheet_name | str | hedef sayfa adı.|
| row | int | hedef satır|
| col | int | hedef sütun|

###  örnekler

Aşağıdaki kod, xml verilerini Cell A1'deki 'Sayfa 1' çalışma sayfasına aktarır.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Bir XML veri dosyasını çalışma kitabına aktarır/günceller.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | xml dosya akışı.|
| sheet_name | str | hedef sayfa adı.|
| row | int | hedef satır.|
| col | int | hedef sütun.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
