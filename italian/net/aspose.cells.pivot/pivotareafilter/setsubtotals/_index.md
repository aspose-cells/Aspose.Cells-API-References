---
title: "PivotAreaFilter.SetSubtotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotAreaFilter. Subtotale per il filtro"
type: docs
url: /it/net/aspose.cells.pivot/pivotareafilter/setsubtotals/
---
## PivotAreaFilter.SetSubtotals method

Subtotale per il filtro.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | La funzione di subtotale. |
| visualizzato | Booleano | Indica se mostra questi dati di subtotale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 8;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Crea un'area pivot con il parametro della tabella pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = new PivotAreaFilter();

            try
            {
                // Chiama SetSubtotals con il tipo di subtotale Sum e impostalo per la visualizzazione
                filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                
                // Verifica se il subtotale è impostato
                bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is set: {isSumSet}");

                // Aggiorna la tabella pivot per vedere le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


