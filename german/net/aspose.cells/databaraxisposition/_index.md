---
title: "Enum DataBarAxisPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBarAxisPosition enum. Gibt die Achsenposition für einen Zellbereich mit bedingter Formatierung als Datenbalken an."
type: docs
url: /de/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Gibt die Achsenposition für einen Zellbereich mit bedingter Formatierung als Datenbalken an.

```csharp
public enum DataBarAxisPosition
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Zeige die Achse an einer variablen Position basierend auf dem Verhältnis des kleinsten negativen Wertes zum größten positiven Wert im Bereich an. Positive Werte werden von links nach rechts angezeigt. Negative Werte werden von rechts nach links angezeigt. Wenn alle Werte positiv oder alle Werte negativ sind, wird keine Achse angezeigt. |
| Midpoint | `1` | Zeige die Achse in der Mitte der Zelle an, unabhängig von den im Bereich vorhandenen Werten. Positive Werte werden von links nach rechts angezeigt. Negative Werte werden von rechts nach links angezeigt. |
| None | `2` | Es wird keine Achse angezeigt, und sowohl positive als auch negative Werte werden von links nach rechts angezeigt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt in der Arbeitsmappe
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hinzufügen einer Regel für bedingte Formatierung
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Festlegen des Bereichs für die bedingte Formatierung
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Hinzufügen einer Datenbalken‑Bedingung
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Festlegen von Eigenschaften für den Datenbalken
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Einsetzen von Zellwerten
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Die Excel-Datei speichern
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


