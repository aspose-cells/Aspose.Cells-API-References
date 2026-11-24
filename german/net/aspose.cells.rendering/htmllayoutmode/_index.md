---
title: "Enum HtmlLayoutMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.HtmlLayoutMode Enum. Stellt den Layoutmodus für HTML-Rendering dar"
type: docs
url: /de/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Stellt den Layoutmodus für das HTML‑Rendern dar.

```csharp
public enum HtmlLayoutMode
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Normal | `0` | Rendert Inhalte wie MS Excel. |
| Print | `1` | Rendert Inhalte im Drucklayoutmodus. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge einige Beispieldaten zum Arbeitsblatt hinzu
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Erstellen Sie HtmlSaveOptions und setzen Sie den Layoutmodus auf Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Speichern Sie die Arbeitsmappe mit normalem Layoutmodus
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Ändern Sie den Layoutmodus auf Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Speichern Sie die Arbeitsmappe mit Druck-Layoutmodus
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Die Enum-Werte anzeigen
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


