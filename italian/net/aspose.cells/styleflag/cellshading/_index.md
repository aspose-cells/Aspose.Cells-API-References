---
title: "StyleFlag.CellShading"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione di ombreggiatura della cella"
type: docs
url: /it/net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

L'impostazione di ombreggiatura della cella sarà applicata.

```csharp
public bool CellShading { get; set; }
```

### Esempi

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

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


