---
title: "StyleFlag.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán los ajustes de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/font/
---
## StyleFlag.Font property

Se aplicarán las configuraciones de fuente.

```csharp
public bool Font { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var shape = workbook.Worksheets[0].Shapes.AddButton(0, 0, 100, 100, 100, 100);
            shape.Text = "Sample Text";
            
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.Name = "Arial";
            font.Size = 14;
            font.Color = Color.Blue;
            font.IsBold = true;
            
            StyleFlag flag = new StyleFlag();
            flag.Font = true;
            
            shape.FormatCharacters(0, shape.Text.Length, font, flag);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


