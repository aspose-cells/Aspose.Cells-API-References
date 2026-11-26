---
title: "StyleFlag.CellShading"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "StyleFlag propiedad. La configuración de sombreado de celda se aplicará"
type: docs
url: /es/net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

Se aplicará la configuración de sombreado de celda.

```csharp
public bool CellShading { get; set; }
```

### Ejemplos

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

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


