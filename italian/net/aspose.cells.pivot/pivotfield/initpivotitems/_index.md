---
title: "PivotField.InitPivotItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField method. Inizializza gli elementi pivot del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/initpivotitems/
---
## PivotField.InitPivotItems method

Inizializza gli elementi pivot del campo pivot

```csharp
[Obsolete("Please simply remove calling this method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void InitPivotItems()
```

### Osservazioni

NOTE: Questo metodo è ora obsoleto. Si prega di rimuovere semplicemente la chiamata a questo metodo. Questo metodo sarà rimosso tra 6 mesi a partire da ottobre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodInitPivotItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Inizializza gli elementi pivot
                pivotField.InitPivotItems();

                // Visualizza gli elementi pivot
                Console.WriteLine("Pivot Items after initialization:");
                foreach (PivotItem item in pivotField.PivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Salva la cartella di lavoro
                workbook.Save("PivotFieldInitPivotItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InitPivotItems method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


