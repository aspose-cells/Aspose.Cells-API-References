---
title: "Shape.ControlData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Daten der Steuerung zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Liest die Daten des Steuerelements.

```csharp
public byte[] ControlData { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Zugriff auf ControlData (schreibgeschützte Eigenschaft)
            byte[] controlData = shape.ControlData;

            // ControlData prüfen
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

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


