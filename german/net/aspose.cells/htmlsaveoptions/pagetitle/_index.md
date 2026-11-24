---
title: "HtmlSaveOptions.PageTitle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream.

```csharp
public string PageTitle { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPageTitleDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            // HTML-Speicheroptionen mit PageTitle festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.PageTitle = "My Custom Page Title";

            // In HTML mit dem angegebenen Titel speichern
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with custom page title: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


