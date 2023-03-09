---
title: default_style fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 540
url: /sv/python-net/aspose.cells/workbook/default_style/
is_root: false
---
##  default_style fastighet

Hämtar eller ställer in standardobjektet [Style](/cells/sv/python-net/aspose.cells/style) för arbetsboken.

###  Anmärkningar

Egenskapen DefaultStyle är användbar för att implementera en stil för hela arbetsboken.

###  Exempel

Följande kod skapar och instansierar en ny arbetsbok och anger standardvärdet [Style](/cells/sv/python-net/aspose.cells/style) för den.

```python
from aspose.cells import Workbook

workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle

```
###  Definition:
```python
@property
def default_style(self):
    ...
@default_style.setter
def default_style(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [Style](/cells/sv/python-net/aspose.cells/style)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
