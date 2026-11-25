---
title: "WorksheetCollection.SortNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Ordina i nomi definiti"
type: docs
url: /it/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Ordina i nomi definiti.

```csharp
public void SortNames()
```

### Osservazioni

Se crei un gran numero di intervalli denominati nel file Excel, chiama questo metodo dopo che tutti gli intervalli denominati sono stati creati e prima di salvare

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni intervalli denominati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Visualizza i nomi prima dell'ordinamento
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Ordina i nomi
            workbook.Worksheets.SortNames();
            
            // Visualizza i nomi dopo l'ordinamento
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


