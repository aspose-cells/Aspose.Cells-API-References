---
title: HorizontalPageBreak sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 750
url: /tr/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak sınıfı
Yatay bir sayfa sonunu temsil eden nesneyi kapsüller.



HorizontalPageBreak türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [start_column](/cells/tr/python-net/aspose.cells/horizontalpagebreak/start_column) | Bu yatay sayfa sonunun başlangıç sütun dizinini alır.|
| [end_column](/cells/tr/python-net/aspose.cells/horizontalpagebreak/end_column) | Bu yatay sayfa sonunun bitiş sütun dizinini alır.|
| [row](/cells/tr/python-net/aspose.cells/horizontalpagebreak/row) | Sıfır tabanlı satır dizinini alır.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
