---
title: "Shape.InputRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene o imposta l'intervallo del foglio di lavoro utilizzato per riempire la casella combinata specificata"
type: docs
url: /it/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Ottiene o imposta l'intervallo del foglio di lavoro usato per riempire la casella combinata specificata.

```csharp
public string InputRange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Aggiungi una forma (rettangolo)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Imposta l'intervallo di input per la forma
            shape.InputRange = "$A$1:$A$5";

            // Verifica e modifica l'intervallo di input se necessario
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


