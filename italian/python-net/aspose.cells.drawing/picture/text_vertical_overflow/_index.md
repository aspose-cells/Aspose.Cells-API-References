---
title: text_vertical_overflow proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1210
url: /it/python-net/aspose.cells.drawing/picture/text_vertical_overflow/
is_root: false
---
##  text_vertical_overflow proprietà

Ottiene e imposta il tipo di overflow verticale del testo della forma che contiene il testo.

###  Esempio

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_vertical_overflow == TextOverflowType.CLIP:
    shape.text_vertical_overflow = TextOverflowType.OVERFLOW

```
###  Definizione:
```python
@property
def text_vertical_overflow(self):
    ...
@text_vertical_overflow.setter
def text_vertical_overflow(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Picture](/cells/it/python-net/aspose.cells.drawing/picture)
* classe [TextOverflowType](/cells/it/python-net/aspose.cells.drawing/textoverflowtype)
