---
title: "PdfSaveOptions.ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt den Bildtyp beim Konvertieren des Diagramms und der Form an"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Gibt den Bildtyp beim Konvertieren des Diagramms und der Form an.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen werden Diagramm und Form immer als Vektorelemente (z. B. Punkt, Linie) für die Renderqualität dargestellt. Diese Eigenschaft wird 12 Monate nach Juni 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstellen Sie ein Beispiel-Arbeitsblatt mit einigen Daten
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // PDF-Speicheroptionen erstellen
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Zeigen Sie den Standardwert von ImageType an
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Legen Sie einen anderen ImageType-Wert fest
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Speichern Sie das Arbeitsbuch als PDF mit dem angegebenen ImageType
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


