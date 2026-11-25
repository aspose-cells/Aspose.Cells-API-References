---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Imposta le proprietà della cartella di lavoro
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Dimostra ExportWorkbookProperties impostandolo su false
            options.ExportWorkbookProperties = false;
            
            // Salva la cartella di lavoro come HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


