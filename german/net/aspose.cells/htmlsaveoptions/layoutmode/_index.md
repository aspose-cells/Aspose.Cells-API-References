---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt den Layoutmodus beim Speichern nach HTML zurück oder legt ihn fest. Der Standardwert ist Normal"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Ruft den Layoutmodus ab oder legt ihn fest, wenn in HTML gespeichert wird. Der Standardwert ist Normal.

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Erstelle eine HtmlSaveOptions-Instanz
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Den aktuellen LayoutMode-Wert anzeigen
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // LayoutMode auf Print setzen
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Speichern Sie die Arbeitsmappe im Drucklayoutmodus
                workbook.Save("LayoutModePrint.html", options);

                // Setzen Sie LayoutMode auf Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Speichern Sie die Arbeitsmappe im normalen Layoutmodus
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


