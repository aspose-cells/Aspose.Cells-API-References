---
title: "Enum DataBarNegativeColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBarNegativeColorType-Enum. Gibt an, ob dieselbe Rand- und Füllfarbe wie bei positiven Datenbalken verwendet werden soll"
type: docs
url: /de/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Gibt an, ob derselbe Rand‑ und Füllfarbton wie bei positiven Datenbalken verwendet werden soll.

```csharp
public enum DataBarNegativeColorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Color | `0` | Verwenden Sie die im Dialogfeld Negative Werte und Achseneinstellungen angegebene Farbe oder indem Sie die Eigenschaften ColorType und BorderColorType des Objekts NegativeBarFormat verwenden. |
| SameAsPositive | `1` | Verwenden Sie dieselbe Farbe wie bei positiven Datenbalken. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Legen Sie die Eigenschaften des Datenbalkens fest
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Legen Sie die Eigenschaften des negativen Balkenformats fest
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


