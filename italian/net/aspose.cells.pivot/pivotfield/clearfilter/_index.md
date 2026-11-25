---
title: "PivotField.ClearFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Cancella l'impostazione del filtro su questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Cancella le impostazioni del filtro su questo campo pivot.

```csharp
public void ClearFilter()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Applica un filtro prima per dimostrare la sua cancellazione
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // Chiama il metodo ClearFilter
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Aggiorna la tabella pivot per mostrare le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


