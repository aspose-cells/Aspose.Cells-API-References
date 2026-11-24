---
title: "PivotArea.IsRowGrandIncluded"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotArea-Eigenschaft. Gibt an, ob die Gesamtsumme der Zeile enthalten ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotarea/isrowgrandincluded/
---
## PivotArea.IsRowGrandIncluded property

Gibt an, ob die Gesamtsumme der Zeile enthalten ist.

```csharp
public bool IsRowGrandIncluded { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsRowGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Felder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Pivot-Format erstellen
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // IsRowGrandIncluded-Eigenschaft demonstrieren
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = false;

            // Stil anwenden, um die Gesamtsumme‑Zeile hervorzuheben
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            workbook.Save("PivotAreaIsRowGrandIncludedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


