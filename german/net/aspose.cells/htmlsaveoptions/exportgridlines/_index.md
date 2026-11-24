---
title: "HtmlSaveOptions.ExportGridLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob die Gitternetzlinien exportiert werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false.

```csharp
public bool ExportGridLines { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportGridLinesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gitternetzlinien-Sichtbarkeit festlegen
            worksheet.IsGridlinesVisible = true;

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportGridLines = worksheet.IsGridlinesVisible,
                ExportActiveWorksheetOnly = true
            };

            // Als HTML speichern
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


