---
title: "HtmlSaveOptions.ExportGridLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le linee della griglia. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Indica se esportare le linee della griglia. Il valore predefinito è false.

```csharp
public bool ExportGridLines { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportGridLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la visibilità delle linee della griglia
            worksheet.IsGridlinesVisible = true;

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportGridLines = worksheet.IsGridlinesVisible,
                ExportActiveWorksheetOnly = true
            };

            // Salva come HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


