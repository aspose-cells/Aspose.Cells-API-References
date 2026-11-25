---
title: "ListObject.EndRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene la riga finale dell'intervallo"
type: docs
url: /it/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Ottiene la riga finale dell'intervallo.

```csharp
public int EndRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Crea oggetto elenco/tabella
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Visualizza EndRow iniziale
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Aggiungi nuova riga alla tabella
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Visualizza EndRow aggiornato
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Salva la cartella di lavoro
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


