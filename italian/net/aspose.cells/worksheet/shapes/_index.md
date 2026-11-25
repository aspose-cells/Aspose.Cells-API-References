---
title: "Worksheet.Shapes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Restituisce tutte le forme di disegno in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Restituisce tutte le forme di disegno in questo foglio di lavoro.

```csharp
public ShapeCollection Shapes { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi alcune forme al foglio di lavoro
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Modifica le proprietà della forma
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Aggiorna le proprietà della prima forma
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


