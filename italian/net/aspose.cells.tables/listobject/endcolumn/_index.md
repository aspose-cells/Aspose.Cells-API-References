---
title: "ListObject.EndColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene la colonna finale dell'intervallo"
type: docs
url: /it/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Ottiene la colonna finale dell'intervallo.

```csharp
public int EndColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Crea un oggetto elenco/tabella
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Visualizza la colonna finale originale
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Ridimensiona la tabella per includere un'altra colonna
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Visualizza la nuova colonna finale
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Salva la cartella di lavoro
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


