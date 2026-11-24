---
title: "Class DataBar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBar class. Beschreibt die DataBar bedingte Formatierungsregel. Diese bedingte Formatierungsregel zeigt einen abgestuften Datenbalken im Zellbereich an."
type: docs
url: /de/net/aspose.cells/databar/
---
## DataBar class

Beschreibt die DataBar‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellenbereich an.

```csharp
public class DataBar
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Liest die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Liest oder setzt die Position der Achse der Datenbalken, die durch eine bedingte Formatierungsregel festgelegt werden. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Liest ein Objekt, das den Rand eines Datenbalkens festlegt. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Liest oder legt fest, wie ein Datenbalken mit Farbe gefüllt wird. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Lese oder setze die Farbe dieses Datenbalkens. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | Liest oder legt die Richtung fest, in der der Datenbalken angezeigt wird. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Lese oder setze das Maximalwert-Objekt dieses Datenbalkens. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Min zugewiesen werden. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Stellt die maximale Länge des Datenbalkens dar. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Lese oder setze das Minimalwert-Objekt dieses Datenbalkens. Es kann nicht null oder ein CFValueObject vom Typ FormatConditionValueType.Max zugewiesen werden. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Stellt die minimale Länge des Datenbalkens dar. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Liest das NegativeBarFormat-Objekt, das mit einer bedingten Formatierungsregel für Datenbalken verknüpft ist. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Lese oder setze das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird. Der Standardwert ist true. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Rendert den Datenbalken in einer Zelle zu einem Bild‑Byte‑Array. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Datenbalken abrufen
            DataBar dataBar = cond.DataBar;

            // Datenbalken‑Eigenschaften festlegen
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Zellwerte einfügen
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Die Excel-Datei speichern
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


