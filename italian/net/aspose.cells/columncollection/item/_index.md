---
title: "ColumnCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColumnCollection. Ottiene un oggetto Column per indice di colonna. L'oggetto Column dell'indice di colonna specificato verrà istanziato se non esiste già"
type: docs
url: /it/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Ottiene un oggetto [`Column`](../../column/) per indice di colonna. L'oggetto Column dell'indice di colonna specificato verrà istanziato se non esiste già.

```csharp
public Column this[int columnIndex] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di colonne
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Imposta la larghezza per le colonne usando la proprietà Item
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Visualizza le larghezze delle colonne
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Verifica che le larghezze delle colonne siano impostate correttamente
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Vedi anche

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


