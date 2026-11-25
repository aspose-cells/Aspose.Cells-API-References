---
title: "PivotTable.RowGrand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se mostrare i totali complessivi per le righe di questa tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/rowgrand/
---
## PivotTable.RowGrand property

Indica se mostrare i totali complessivi per le righe di questa tabella pivot.

```csharp
[Obsolete("Use PivotTable.ShowRowGrandTotals property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool RowGrand { get; set; }
```

### Osservazioni

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.ShowRowGrandTotals. Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRowGrandDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            
            worksheet.Cells["A5"].PutValue("Product A");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(1500);
            
            worksheet.Cells["A6"].PutValue("Product B");
            worksheet.Cells["B6"].PutValue("North");
            worksheet.Cells["C6"].PutValue(2500);

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C6", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di RowGrand
            Console.WriteLine("Current RowGrand value: " + pivotTable.RowGrand);

            // Modifica la proprietà RowGrand
            pivotTable.RowGrand = false;

            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePropertyRowGrandDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


