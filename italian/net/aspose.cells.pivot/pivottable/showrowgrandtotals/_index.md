---
title: "PivotTable.ShowRowGrandTotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se mostrare i totali complessivi per le righe della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Indica se mostrare i totali complessivi per le righe della tabella pivot.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowGrandTotalsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product A";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product B";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            
            cells["A4"].Value = "Product A";
            cells["B4"].Value = "South";
            cells["C4"].Value = 2000;
            
            cells["A5"].Value = "Product B";
            cells["B5"].Value = "North";
            cells["C5"].Value = 1200;

            // Aggiungi una tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Configura la tabella pivot
            pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
            pivotTable.ShowColumnGrandTotals = true;
            
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


