---
title: "Style.BackgroundArgbColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits"
type: docs
url: /fr/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


