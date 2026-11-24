---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt die Gitterlinienfarbe zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Liest oder legt die Farbe der Gitternetzlinien fest.

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
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // PDF-Speicheroptionen erstellen
                PdfSaveOptions options = new PdfSaveOptions();

                // Standardwert von GridlineColor anzeigen
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Neue Gitterlinienfarbe festlegen
                options.GridlineColor = Color.Red;

                // Aktualisierten GridlineColor-Wert anzeigen
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Speichern Sie die Arbeitsmappe mit der Einstellung für die Gitterlinienfarbe
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


