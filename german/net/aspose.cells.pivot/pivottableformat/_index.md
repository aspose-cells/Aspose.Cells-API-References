---
title: "Klasse PivotTableFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableFormat Klasse. Stellt das im PivotTable definierte Format dar"
type: docs
url: /de/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

Stellt das im PivotTable definierte Format dar.

```csharp
public class PivotTableFormat
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Ruft den Pivot-Bereich ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Ruft den formatierten Stil ab. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Setzt den Stil des Pivot-Bereichs. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Greife auf die PivotTableFormatCollection zu
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Ein neues Format zur Sammlung hinzufügen
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Zugriff auf den PivotArea des Formats
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Erstelle einen neuen Stil
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Den Stil auf das PivotTableFormat anwenden
            pivotFormat.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


