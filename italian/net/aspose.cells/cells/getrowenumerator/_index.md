---
title: "Cells.GetRowEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'enumeratore delle righe"
type: docs
url: /it/net/aspose.cells/cells/getrowenumerator/
---
## Cells.GetRowEnumerator method

Ottiene l'enumeratore delle righe.

```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```

### Valore di ritorno

L'enumeratore delle righe.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo RowCollection.GetEnumerator(). Questo metodo sarà rimosso 12 mesi dopo da maggio 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetRowEnumeratorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Row 1 Data");
            worksheet.Cells["A3"].PutValue("Row 3 Data");
            worksheet.Cells["A5"].PutValue("Row 5 Data");

            try
            {
                // Ottieni l'enumeratore delle righe dalla raccolta Cells
                IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
                
                Console.WriteLine("Iterating through rows containing data:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Cell cell = row.GetCellOrNull(0); // Get first cell in row
                    string cellValue = cell != null ? cell.Value.ToString() : "empty";
                    Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


