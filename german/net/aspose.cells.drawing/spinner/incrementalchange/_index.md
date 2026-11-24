---
title: "Spinner.IncrementalChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Spinner-Eigenschaft. Gibt die Menge zurück, um die die Bildlaufleiste oder der Spinner bei einem Zeilen-Scroll erhöht wird, oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Liest oder legt den Betrag fest, um den die Bildlaufleiste oder der Spinner bei einem Zeilen-Scroll erhöht wird.

```csharp
public int IncrementalChange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Spinner-Steuerelement
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Spinner-Eigenschaften festlegen
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Überprüfe und gib den IncrementalChange-Wert aus
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Ändere und überprüfe erneut
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Speichere die Arbeitsmappe
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


