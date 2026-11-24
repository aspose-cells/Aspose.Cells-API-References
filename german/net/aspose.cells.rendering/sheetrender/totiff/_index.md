---
title: "SheetRender.ToTiff"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Methode. Rendert das gesamte Arbeitsblatt als Tiff-Bild in einen Stream"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Ganzes Arbeitsblatt als Tiff‑Bild in einen Stream rendern.

```csharp
public void ToTiff(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | der Stream des Ausgabebildes |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielinhalt hinzufügen, um das Rendern zu demonstrieren
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Bildoptionen für das Rendern konfigurieren
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Erstellen Sie einen SheetRenderer mit konfigurierten Optionen
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Ausgabestream für TIFF-Bild erstellen
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Arbeitsblatt mit Stream in TIFF rendern
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Ganzes Arbeitsblatt als Tiff‑Bild in eine Datei rendern.

```csharp
public void ToTiff(string filename)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | String | der Dateiname des Ausgabebildes |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Lade die Quell-Excel-Datei
            Workbook workbook = new Workbook("Book1.xlsx");

            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Erstelle SheetRender für das erste Arbeitsblatt
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Alle Seiten des Blatts als mehrseitige TIFF-Datei speichern
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


