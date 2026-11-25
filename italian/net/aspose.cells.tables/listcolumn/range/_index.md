---
title: "ListColumn.Range"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListColumn. Ottiene l'intervallo di questa colonna dell'elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Ottiene l'intervallo di questa colonna dell'elenco.

```csharp
public Range Range { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare un oggetto elenco
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Crea un oggetto elenco
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Ottieni la prima colonna dell'elenco
            ListColumn listCol = listObj.ListColumns[0];
            
            // Accedi all'intervallo della colonna dell'elenco
            Aspose.Cells.Range range = listCol.Range;
            
            // Visualizza le informazioni sull'intervallo
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Modifica le celle nell'intervallo
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


