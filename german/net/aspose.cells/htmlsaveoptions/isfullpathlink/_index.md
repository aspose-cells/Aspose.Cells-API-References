---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob ein Vollpfad-Link in sheet00x.htmfilelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Gibt an, ob ein Vollpfad‑Link in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demonstriere die IsFullPathLink-Eigenschaft
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Speichern mit unterschiedlichen IsFullPathLink-Einstellungen
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


