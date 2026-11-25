---
title: "Shape.HasLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta la visibilità del bordo della linea della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Ottiene e imposta se il bordo della forma è visibile.

```csharp
public bool HasLine { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Dimostra la proprietà HasLine
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Rimuovi la linea
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Aggiungi nuovamente la linea
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


