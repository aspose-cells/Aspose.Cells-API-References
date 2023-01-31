---
title: default_style property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 540
url: /python-net/aspose.cells/workbook/default_style/
is_root: false
---

## default_style property


Gets or sets the default [Style](/cells/python-net/aspose.cells/style) object of the workbook.
### Remarks 


The DefaultStyle property is useful to implement a Style for the whole Workbook.
### Example 


The following code creates and instantiates a new Workbook and sets a default [Style](/cells/python-net/aspose.cells/style) to it.

```
from aspose.cells import Workbook

workbook = Workbook()
defaultStyle = workbook.default_style
defaultStyle.font.name = "Tahoma"
workbook.default_style = defaultStyle

```

### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
