---
title: "Shape.ControlData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene i dati del controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Ottiene i dati del controllo.

```csharp
public byte[] ControlData { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Accedi a ControlData (proprietà di sola lettura)
            byte[] controlData = shape.ControlData;

            // Verifica ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


