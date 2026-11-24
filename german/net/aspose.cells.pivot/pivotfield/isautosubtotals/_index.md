---
title: "PivotField.IsAutoSubtotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField‑Eigenschaft. Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist true."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Gibt an, ob das angegebene Feld automatische Zwischensummen anzeigt. Standard ist wahr.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
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

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Fügen Sie ein Feld zum Zeilenbereich hinzu und setzen Sie IsAutoSubtotals auf false.
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.IsAutoSubtotals = false; // Disable automatic subtotals

            // Fügen Sie ein Feld zum Datenbereich hinzu.
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Daten berechnen
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldIsAutoSubtotalsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


