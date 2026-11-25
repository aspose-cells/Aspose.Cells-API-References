---
title: "PivotTable.PrintDrill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti espandi/collassa quando visualizzati nella tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati. Stampa i pulsanti di espansione/collasso quando visualizzati nella tabella pivot.

```csharp
public bool PrintDrill { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintDrillDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Cars";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bikes";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 2500;

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Dimostra la proprietà PrintDrill
            pivotTable.PrintDrill = false; // Disable printing drill indicators
            pivotTable.ShowDrill = true;   // Show drill indicators on screen
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePrintDrillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


