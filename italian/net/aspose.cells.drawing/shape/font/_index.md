---
title: "Shape.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta il font della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/font/
---
## Shape.Font property

Rappresenta il carattere della forma.

```csharp
public Font Font { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Accedi e modifica le proprietà del font della forma
            Aspose.Cells.Font font = shape.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("ShapeFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


