---
title: "StyleFlag.CellShading"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för cellskuggning kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

Inställning för cellskuggning kommer att tillämpas.

```csharp
public bool CellShading { get; set; }
```

### Exempel

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

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


