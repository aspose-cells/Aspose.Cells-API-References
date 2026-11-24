---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper property. Liest und schreibt die Vordergrundfarbe der Füllung"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Liest und setzt die Vordergrundfarbe der Füllung.

```csharp
public Color ForeColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Label hinzu, um das Beispiel sinnvoll zu machen
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Erstelle eine Instanz von MsoFillFormatHelper mittels Reflexion (kein öffentlicher Konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Zeige den Standardwert von ForeColor an
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Setze einen neuen ForeColor-Wert
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Demonstriere das Abrufen des ForeColor-Werts
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Speichern Sie die Arbeitsmappe, um die erfolgreiche Ausführung zu demonstrieren
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


