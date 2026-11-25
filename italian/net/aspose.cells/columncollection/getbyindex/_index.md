---
title: "ColumnCollection.GetByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ColumnCollection. Ottiene l'oggetto column per indice"
type: docs
url: /it/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Ottiene l'oggetto column per indice.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 |  |

### Valore di ritorno

Restituisce l'oggetto column.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Columns.GetColumnByIndex(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2010. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea colonne nella raccolta impostando le larghezze
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Ottieni la seconda colonna da ColumnCollection (indice 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Modifica la colonna recuperata
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


