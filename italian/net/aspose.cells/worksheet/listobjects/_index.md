---
title: "Worksheet.ListObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene tutti i ListObjects in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Ottiene tutti i ListObjects in questo foglio di lavoro.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Crea un ListObject (tabella)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Ridimensiona la tabella per includere più righe
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Aggiungi più dati alla tabella estesa
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Accedi alla tabella tramite la proprietà ListObjects
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Salva la cartella di lavoro
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


