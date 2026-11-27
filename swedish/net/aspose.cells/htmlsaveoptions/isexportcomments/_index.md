---
title: "HtmlSaveOptions.IsExportComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om kommentarer exporteras när filen sparas som html. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Anger om kommentarer ska exporteras när filen sparas i HTML, standardvärdet är false.

```csharp
public bool IsExportComments { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExportCommentsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata och kommentarer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Lägg till en kommentar
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            
            // Spara med IsExportComments = false (kommentarer kommer inte att exporteras)
            HtmlSaveOptions options1 = new HtmlSaveOptions
            {
                IsExportComments = false
            };
            workbook.Save("output_without_comments.html", options1);
            
            // Spara med IsExportComments = true (kommentarer kommer att exporteras)
            HtmlSaveOptions options2 = new HtmlSaveOptions
            {
                IsExportComments = true
            };
            workbook.Save("output_with_comments.html", options2);
            
            Console.WriteLine("HTML files created successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


