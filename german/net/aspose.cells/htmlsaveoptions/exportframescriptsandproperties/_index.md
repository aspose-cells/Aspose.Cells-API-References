---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // HTML‑Speicheroptionen mit ExportFrameScriptsAndProperties festlegen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // Als HTML speichern
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


