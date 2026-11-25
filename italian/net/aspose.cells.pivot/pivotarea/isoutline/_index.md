---
title: "PivotArea.IsOutline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotArea. Indica se la regola si riferisce a un'area che è in modalità outline"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Indica se la regola si riferisce a un'area in modalità struttura.

```csharp
public bool IsOutline { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Crea e configura PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


