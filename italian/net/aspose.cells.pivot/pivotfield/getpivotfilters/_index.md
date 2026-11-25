---
title: "PivotField.GetPivotFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Ottiene i filtri pivot del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getpivotfilters/
---
## PivotField.GetPivotFilters method

Ottiene i filtri pivot del campo pivot

```csharp
[Obsolete("Use PivotField.GetFilters() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetPivotFilters()
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFilters(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotFieldMethodGetPivotFiltersDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Chiama il metodo GetPivotFilters (obsoleto)
                ArrayList pivotFilters = pivotField.GetPivotFilters();
                
                Console.WriteLine($"Number of pivot filters: {pivotFilters.Count}");
                
                // In alternativa, utilizza il metodo GetFilters() non obsoleto
                PivotFilter[] filters = pivotField.GetFilters();
                Console.WriteLine($"Number of filters (non-obsolete method): {filters.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPivotFilters method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetPivotFiltersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


