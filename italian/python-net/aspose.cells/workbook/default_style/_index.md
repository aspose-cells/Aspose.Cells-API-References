---
title: default_style proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 540
url: /it/python-net/aspose.cells/workbook/default_style/
is_root: false
---
##  default_style proprietà

Ottiene o imposta l'oggetto [Style](/cells/it/python-net/aspose.cells/style) predefinito della cartella di lavoro.

###  Osservazioni

La proprietà DefaultStyle è utile per implementare uno stile per l'intera cartella di lavoro.

###  Esempio

Il codice seguente crea e crea un'istanza di una nuova cartella di lavoro e ne imposta un valore predefinito [Style](/cells/it/python-net/aspose.cells/style).

```python
from aspose.cells import Workbook

workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle

```
###  Definizione:
```python
@property
def default_style(self):
    ...
@default_style.setter
def default_style(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Style](/cells/it/python-net/aspose.cells/style)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
