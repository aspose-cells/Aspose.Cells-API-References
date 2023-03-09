---
title: VerticalPageBreak klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1560
url: /sv/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak klass
Kapslar in objektet som representerar en vertikal sidbrytning.



Typen VerticalPageBreak avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [start_row](/cells/sv/python-net/aspose.cells/verticalpagebreak/start_row) | Hämtar startradindex för den vertikala sidbrytningen.|
| [end_row](/cells/sv/python-net/aspose.cells/verticalpagebreak/end_row) | Hämtar slutradens index för den vertikala sidbrytningen.|
| [column](/cells/sv/python-net/aspose.cells/verticalpagebreak/column) | Hämtar kolumnindex för den vertikala sidbrytningen.|



###  Exempel

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Se även
* modul [aspose.cells](..)
