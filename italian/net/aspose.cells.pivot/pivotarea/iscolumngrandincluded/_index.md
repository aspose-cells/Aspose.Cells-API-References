---
title: "PivotArea.IsColumnGrandIncluded"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotArea. Indica se il totale generale della colonna è incluso"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/iscolumngrandincluded/
---
## PivotArea.IsColumnGrandIncluded property

Indica se il totale generale della colonna è incluso.

```csharp
public bool IsColumnGrandIncluded { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsColumnGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configura l'area pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.RuleType = PivotAreaType.Normal;

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


