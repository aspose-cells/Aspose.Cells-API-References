---
title: "CellWatch.CellName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CellWatch proprietà. Ottiene e imposta il nome della cella"
type: docs
url: /it/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Ottiene e imposta il nome della cella.

```csharp
public string CellName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni monitor di celle
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Visualizza i nomi delle celle di tutti i monitor
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Aggiungi un nuovo monitor e visualizza il suo nome
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Salva la cartella di lavoro
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


