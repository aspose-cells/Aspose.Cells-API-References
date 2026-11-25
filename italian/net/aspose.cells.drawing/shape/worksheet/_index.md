---
title: "Shape.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene l'oggetto Worksheet che contiene questa forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Ottiene l'oggetto [`Worksheet`](../../../aspose.cells/worksheet/) che contiene questa forma.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Dimostrare l'uso della proprietà Worksheet
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Visualizza il nome del foglio di lavoro per dimostrare che la proprietà funziona
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


