---
title: Aspose::Cells::Workbook::GetDefaultStyle method
linktitle: GetDefaultStyle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Workbook::GetDefaultStyle method. Gets or sets the default Style object of the workbook in C++.'
type: docs
weight: 3000
url: /cpp/aspose.cells/workbook/getdefaultstyle/
---
## Workbook::GetDefaultStyle method


Gets or sets the default [Style](../../style/) object of the workbook.

```cpp
Style Aspose::Cells::Workbook::GetDefaultStyle()
```

## Remarks


The DefaultStyle property is useful to implement a [Style](../../style/) for the whole [Workbook](../). 

## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook;
Style defaultStyle = workbook.GetDefaultStyle();
defaultStyle.GetFont().SetName(u"Tahoma");
workbook.SetDefaultStyle(defaultStyle);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Style](../../style/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
