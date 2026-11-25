---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo viene aperto"
type: docs
url: /it/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Rappresenta il nome del foglio di lavoro attivo quando il foglio elettronico viene aperto.

```csharp
public string ActiveSheetName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Imposta il foglio attivo per nome
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Verifica il foglio attivo
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


