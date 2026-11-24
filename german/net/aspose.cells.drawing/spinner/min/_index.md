---
title: "Spinner.Min"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Spinner-Eigenschaft. Gibt den Minimalwert einer Bildlaufleiste oder eines Spinnerbereichs zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Liest oder legt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs fest.

```csharp
public int Min { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Spinner-Steuerelement mit den richtigen Abmessungen hinzu
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Setzen Sie Spinner-Eigenschaften einschließlich Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Überprüfen und geben Sie die Min-Eigenschaft aus
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Speichere die Arbeitsmappe
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


