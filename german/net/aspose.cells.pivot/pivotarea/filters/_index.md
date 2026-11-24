---
title: "PivotArea.Filters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotArea-Eigenschaft. Gibt alle Filter für diesen PivotArea zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/filters/
---
## PivotArea.Filters property

Liest alle Filter für diesen PivotArea.

```csharp
public PivotAreaFilterCollection Filters { get; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyFiltersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "SalesData";
            
            // Erstelle Beispieldaten
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Revenue");
            dataSheet.Cells["A2"].PutValue("Electronics");
            dataSheet.Cells["B2"].PutValue(1500);
            dataSheet.Cells["A3"].PutValue("Furniture");
            dataSheet.Cells["B3"].PutValue(800);
            dataSheet.Cells["A4"].PutValue("Electronics");
            dataSheet.Cells["B4"].PutValue(2200);

            // Pivot-Tabelle erstellen
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Zeilenfeld mit Zwischensummen konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");

            // Pivot-Bereich erstellen und Felder auswählen
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
            pivotArea.SelectField(PivotFieldType.Row, "Category");

            // Verwendung der Filters-Eigenschaft demonstrieren
            Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
            if (pivotArea.Filters.Count > 1)
            {
                bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
                Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
            }

            workbook.Save("PivotFiltersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


