---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se utilizzare link con percorso completo in sheet00x.htmfilelist.xml e tabstrip.htm. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Dimostra la proprietà IsFullPathLink
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Salva con impostazioni diverse di IsFullPathLink
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


