---
title: "HtmlSaveOptions.ExportSingleTab"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare la singola scheda quando il file ha solo un foglio di lavoro. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Indica se esportare la singola scheda quando il file ha solo un foglio di lavoro. Il valore predefinito è false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSingleTabDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con dati di prova
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea le opzioni di salvataggio HTML con ExportSingleTab impostato su true
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportSingleTab = true,
                ExportImagesAsBase64 = true
            };

            // Salva la cartella di lavoro come HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


