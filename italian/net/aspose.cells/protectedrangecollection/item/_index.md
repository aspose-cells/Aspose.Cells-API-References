---
title: "ProtectedRangeCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ProtectedRangeCollection. Ottiene l'elemento ProtectedRange all'indice specificato"
type: docs
url: /it/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Ottiene l'elemento [`ProtectedRange`](../../protectedrange/) all'indice specificato.

```csharp
public ProtectedRange this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un intervallo protetto usando gli indici di cella (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Accedi all'intervallo protetto usando la proprietà Item (indice 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Verifica e visualizza lo stato di protezione
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


