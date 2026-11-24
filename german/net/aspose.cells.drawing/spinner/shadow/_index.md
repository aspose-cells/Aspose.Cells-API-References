---
title: "Spinner.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Spinner-Eigenschaft. Gibt an, ob das Shape eine 3D-Schattierung hat"
type: docs
url: /de/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Gibt an, ob die Form 3‑D‑Schattierung hat.

```csharp
public bool Shadow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einen Spinner zum Arbeitsblatt hinzu
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Spinner-Eigenschaften festlegen
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Shadow-Eigenschaft demonstrieren
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Speichere die Arbeitsmappe
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe, um die Schatten-Eigenschaft zu überprüfen
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Siehe auch

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


