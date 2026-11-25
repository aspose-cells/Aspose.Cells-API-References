---
title: "Workbook.FileName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene e imposta il nome file corrente"
type: docs
url: /it/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Ottiene e imposta il nome file corrente.

```csharp
public string FileName { get; set; }
```

### Osservazioni

Se il file è aperto tramite stream e ci sono riferimenti a formule esterne, impostare il nome file.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Imposta la proprietà nome file
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Aggiungi alcuni dati per dimostrare la funzionalità
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Salva la cartella di lavoro
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Dimostra la modifica del nome file
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Dimostra l'uso di collegamenti esterni
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


