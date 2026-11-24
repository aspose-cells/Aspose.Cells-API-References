---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper-Eigenschaft. Gibt an, ob eine Füllung vorhanden ist"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Gibt an, ob eine Füllung vorhanden ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Label hinzu, um das Beispiel sinnvoll zu machen
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Erstelle eine Instanz von MsoFillFormatHelper mittels Reflexion (kein öffentlicher Konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Zeigen Sie den Standardwert von IsVisible an
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Setzen Sie IsVisible auf true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Setzen Sie IsVisible auf false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Lesen Sie den aktuellen Wert von IsVisible
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Speichern Sie die Arbeitsmappe, um die erfolgreiche Ausführung zu demonstrieren
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


