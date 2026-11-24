---
title: "MsoFillFormatHelper.BackColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper property. Liest und schreibt die Hintergrundfarbe"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Liest und setzt die Hintergrundfarbe der Füllung.

```csharp
public Color BackColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Label hinzu, nur um etwas Inhalt im Blatt zu haben
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper stellt keinen öffentlichen Konstruktor bereit, verwende Reflection, um es zu instanziieren
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Setze die BackColor auf eine bekannte Farbe (z. B. LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Lese den BackColor-Wert aus und zeige ihn an
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Optional kannst du auch den ForeColor auslesen, um zu zeigen, dass er standardmäßig bleibt
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Speichere die Arbeitsmappe – der fill helper ist nicht an eine Form angehängt,
                // aber das Speichern zeigt, dass der Code ohne Fehler ausgeführt wurde.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


