---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeHtmlSaveOptions Eigenschaft. Die allgemeinen Optionen zum Speichern von HTML"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

Die allgemeinen Optionen zum Speichern von HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Hinweise

Wenn eine [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) Instanz angegeben ist, wird das [`SaveFormat`](../saveformat/) überschrieben (falls es zuvor angegeben wurde).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Low-Code HTML-Speicheroptionen erstellen
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Aktuelle Export-Einstellung für Rasterlinien anzeigen
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Mit sichtbaren Rasterlinien speichern
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // HTML-Optionen ändern, um Rasterlinien auszublenden
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Ohne Rasterlinien speichern
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


