---
title: "StyleFlag.CellShading"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Zellschattierungseinstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

Die Einstellung für die Zellen-Schattierung wird angewendet.

```csharp
public bool CellShading { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyCellShadingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            StyleFlag flag = new StyleFlag();
            flag.CellShading = true;
            
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Cell Shading");
            
            cells.ApplyStyle(style, flag);
            
            workbook.Save("CellShadingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


