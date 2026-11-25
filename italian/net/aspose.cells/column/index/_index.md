---
title: "Column.Index"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Ottiene l'indice di questa colonna"
type: docs
url: /it/net/aspose.cells/column/index/
---
## Column.Index property

Restituisce l'indice di questa colonna.

```csharp
public int Index { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle colonne
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // Ottieni la raccolta di colonne
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Dimostra la proprietà Index
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // Accedi alla colonna per indice
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // Modifica la larghezza della colonna usando l'indice
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


