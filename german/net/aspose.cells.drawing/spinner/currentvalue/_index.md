---
title: "Spinner.CurrentValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Spinner-Eigenschaft. Gibt den aktuellen Wert zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Liest oder legt den aktuellen Wert fest.

```csharp
public int CurrentValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Spinner-Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Spinner-Eigenschaften festlegen
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Überprüfen und geben Sie den aktuellen Wert aus
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Speichere die Arbeitsmappe
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


