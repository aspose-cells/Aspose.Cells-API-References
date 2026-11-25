---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le intestazioni di pagina"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Indica se esportare le intestazioni di pagina.

```csharp
public bool ExportPageFooters { get; set; }
```

### Osservazioni

Funziona solo quando [`SaveAsSingleFile`](../saveassinglefile/) è True.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta ExportPageFooters a true per includere i piè di pagina nell'output
            saveOptions.ExportPageFooters = true;
            
            // Imposta le altre opzioni necessarie
            saveOptions.ExportPageHeaders = true;
            
            // Salva la cartella di lavoro in HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


