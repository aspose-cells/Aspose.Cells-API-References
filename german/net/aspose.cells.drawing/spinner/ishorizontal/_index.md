---
title: "Spinner.IsHorizontal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Spinner-Eigenschaft. Gibt an, ob dies eine horizontale Bildlaufleiste ist"
type: docs
url: /de/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Gibt an, ob es sich um eine horizontale Bildlaufleiste handelt.

```csharp
public bool IsHorizontal { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Fügen Sie dem Arbeitsblatt ein Spinner-Shape hinzu
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Spinner-Eigenschaften festlegen
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Demonstrieren Sie die IsHorizontal-Eigenschaft (lesen und schreiben)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Schalten Sie die Ausrichtung um
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Speichere die Arbeitsmappe
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


