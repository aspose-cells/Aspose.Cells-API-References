---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto"
type: docs
url: /it/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Rappresenta l'indice del foglio di lavoro attivo quando il foglio elettronico viene aperto.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Osservazioni

L'indice del foglio parte da zero.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con 3 fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Imposta l'indice del foglio attivo a 1 (secondo foglio)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Verifica il foglio attivo
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Salva la cartella di lavoro
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


