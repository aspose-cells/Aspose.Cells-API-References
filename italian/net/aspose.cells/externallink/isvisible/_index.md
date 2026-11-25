---
title: "ExternalLink.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExternalLink property. Indica se questo collegamento esterno è visibile in MS Excel"
type: docs
url: /it/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indica se questo collegamento esterno è visibile in MS Excel.

```csharp
public bool IsVisible { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un workbook con collegamenti esterni
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Crea un nuovo foglio di lavoro da utilizzare come fonte del collegamento esterno
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Aggiungi un riferimento a un collegamento esterno
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Verifica i collegamenti esterni (verranno creati automaticamente durante il caricamento delle formule)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Crea un altro foglio di lavoro per dimostrare il caricamento di un file esistente
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Salva e ricarica per dimostrare i collegamenti esterni
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Verifica i collegamenti esterni nel foglio di lavoro caricato
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


