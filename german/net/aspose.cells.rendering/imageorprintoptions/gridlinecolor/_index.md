---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die Gitterlinienfarbe zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Ruft die gridline colr ab oder legt sie fest.

```csharp
public Color GridlineColor { get; set; }
```

### Hinweise

Sie ignoriert die Gitterlinienfarbeneinstellungen in der Quelldatei.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten ein, damit das Arbeitsblatt Inhalt hat
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Erstelle eine Instanz von ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Den aktuellen GridlineColor-Wert anzeigen (schreibgeschützt oder lesbar/eschreibbar)
                // Der Eigenschaftstyp wird als System.Drawing.Color angenommen
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Optional das Blatt in ein Bild rendern, um die Auswirkung der Standard‑Gitterlinienfarbe zu sehen
                // (Kein Bedarf, den Wert zu ändern; wir demonstrieren nur die Verwendung.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Arbeitsmappe speichern (optional)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


