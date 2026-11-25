---
title: "HtmlSaveOptions.ExportDataOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica la regola di esportazione dei dati del file HTML. Il valore predefinito è All"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Indica la regola di esportazione dei dati del file html. Il valore predefinito è All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDataOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea le opzioni di salvataggio HTML e imposta ExportDataOptions
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

            // Salva come HTML con tutte le opzioni di esportazione dei dati
            workbook.Save("output.html", htmlSaveOptions);

            Console.WriteLine("HTML file saved with ExportDataOptions.All");
        }
    }
}
```

### Vedi anche

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


