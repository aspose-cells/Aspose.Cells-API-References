---
title: copy yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Bir kaynak aralıktan verileri (formüller dahil), biçimlendirmeyi, çizim nesnelerini vb. kopyalar.



```python
def copy(self, range):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| range | [Range](/cells/tr/python-net/aspose.cells/range) | Kaynak [Range](/cells/tr/python-net/aspose.cells/range) nesnesi.|

###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  copy(range, options) {#Range-PasteOptions}
Özel seçenekleri yapıştırarak aralığı kopyalama.



```python
def copy(self, range, options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| range | [Range](/cells/tr/python-net/aspose.cells/range) | Kaynak aralığı.|
| options | [PasteOptions](/cells/tr/python-net/aspose.cells/pasteoptions) | Yapıştır özel seçenekler.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
