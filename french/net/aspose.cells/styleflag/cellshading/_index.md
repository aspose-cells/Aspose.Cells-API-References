---
title: "StyleFlag.CellShading"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le réglage d'ombrage de cellule sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/cellshading/
---
## StyleFlag.CellShading property

Le paramètre d’ombrage de cellule sera appliqué.

```csharp
public bool CellShading { get; set; }
```

### Exemples

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

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


