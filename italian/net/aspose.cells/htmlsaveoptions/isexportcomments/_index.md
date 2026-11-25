---
title: "HtmlSaveOptions.IsExportComments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indica se esportare i commenti durante il salvataggio del file in HTML, il valore predefinito è false.

```csharp
public bool IsExportComments { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio e commenti
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Aggiungi un commento
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            
            // Salva con IsExportComments = false (i commenti non saranno esportati)
            HtmlSaveOptions options1 = new HtmlSaveOptions
            {
                IsExportComments = false
            };
            workbook.Save("output_without_comments.html", options1);
            
            // Salva con IsExportComments = true (i commenti saranno esportati)
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

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


