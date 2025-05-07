---
title: StyleFlag.Borders
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All borders settings will be applied
type: docs
url: /net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

All borders settings will be applied.

```csharp
public bool Borders { get; set; }
```

### Examples

```csharp
// Called: sflag.Borders = true;
[Test, Ignore("Not ready to test this yet")]
        public void Property_Borders()
        {
            caseName = "testApplyColumnStyle_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = getStyle(workbook);
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;
            cells.ApplyColumnStyle(-1, style, sflag);
            string msg = message + "cells.ApplyColumnStyle(-1, style, sflag)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


