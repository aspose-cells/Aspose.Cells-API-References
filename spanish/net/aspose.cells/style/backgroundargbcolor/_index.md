---
title: "Style.BackgroundArgbColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene y establece el color de fondo con un valor ARGB de 32 bits"
type: docs
url: /es/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Obtiene y establece el color de fondo con un valor ARGB de 32 bits.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Ejemplos

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

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


