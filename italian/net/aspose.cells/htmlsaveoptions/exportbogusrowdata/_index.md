---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare dati di riga finale falsi. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Indica se esportare dati falsi della riga inferiore. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // Prima esportazione senza dati di riga falsi
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Poi esporta con dati di riga falsi
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Visualizza i risultati
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


