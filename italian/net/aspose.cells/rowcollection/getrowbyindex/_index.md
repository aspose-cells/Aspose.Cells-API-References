---
title: "RowCollection.GetRowByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RowCollection. Restituisce l'oggetto riga in base alla posizione nella lista"
type: docs
url: /it/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Restituisce l'oggetto riga in base alla posizione nella lista.

```csharp
public Row GetRowByIndex(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | La posizione. |

### Valore di ritorno

L'oggetto Row nella posizione specificata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ottieni la riga per indice (basato su 0)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### Vedi anche

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


