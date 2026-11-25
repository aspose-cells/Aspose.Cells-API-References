---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Indica se esportare le proprietà del documento. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcune proprietà del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Aggiungi dati di cella di esempio
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Crea le opzioni di salvataggio HTML e imposta ExportDocumentProperties su false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Salva la cartella di lavoro come HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


