---
title: "PivotFilterCollection.ClearFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Rimuove il PivotFilter dal PivotField specifico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/clearfilter/
---
## PivotFilterCollection.ClearFilter method

Cancella il PivotFilter dal PivotField specifico

```csharp
public void ClearFilter(int fieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | l'indice del PivotField |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodClearFilterWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi filtro alla tabella pivot
            PivotFilterCollection filters = pivotTable.PivotFilters;
            filters.AddLabelFilter(0, PivotFilterType.Count, "Apple", null);

            try
            {
                // Chiama il metodo ClearFilter con il parametro indice del campo
                filters.ClearFilter(0);
                
                Console.WriteLine("Pivot filter cleared successfully for field index 0");
                
                // Verifica che il filtro sia stato rimosso
                Console.WriteLine($"Number of filters after clearing: {filters.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterCollectionMethodClearFilterWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


