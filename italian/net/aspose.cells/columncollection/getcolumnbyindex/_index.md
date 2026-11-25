---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ColumnCollection. Ottiene l'oggetto Column in base alla posizione nella lista"
type: docs
url: /it/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Ottiene l'oggetto [`Column`](../../column/) in base alla posizione nella lista.

```csharp
public Column GetColumnByIndex(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | La posizione nella lista. |

### Valore di ritorno

Restituisce l'oggetto column.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alla colonna A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Ottieni il riferimento alla collezione di colonne
                ColumnCollection columns = worksheet.Cells.Columns;

                // Accedi alla colonna all'indice 0 (colonna A) usando GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // Modifica la larghezza della colonna per dimostrare l'accesso alla colonna
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


