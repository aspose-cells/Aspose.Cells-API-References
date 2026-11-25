---
title: "Workbook.Worksheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene la collezione WorksheetCollection nel foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Ottiene la collezione [`WorksheetCollection`](../../worksheetcollection/) nel foglio di calcolo.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Valore di ritorno

[`WorksheetCollection`](../../worksheetcollection/) collection

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Aggiungi un nuovo foglio di lavoro
            workbook.Worksheets.Add("SecondSheet");
            
            // Accedi al secondo foglio di lavoro e aggiungi dati
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Salva la cartella di lavoro
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Restituisci il conteggio dei fogli di lavoro
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


