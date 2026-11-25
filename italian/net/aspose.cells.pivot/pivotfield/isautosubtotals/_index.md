---
title: "PivotField.IsAutoSubtotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Indica se il campo specificato mostra subtotali automatici. Il valore predefinito è true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSubtotalsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi il campo all'area delle righe e imposta IsAutoSubtotals su false
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.IsAutoSubtotals = false; // Disable automatic subtotals

            // Aggiungi il campo all'area dei dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcola i dati
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


