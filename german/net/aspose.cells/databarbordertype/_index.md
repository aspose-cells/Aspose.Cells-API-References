---
title: "Enum DataBarBorderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DataBarBorderType-Enum. Gibt den Randtyp einer Datenleiste an."
type: docs
url: /de/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Gibt den Randtyp eines Datenbalkens an.

```csharp
public enum DataBarBorderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Die Datenleiste hat keinen Rand. |
| Solid | `1` | Die Datenleiste hat einen durchgezogenen Rand. |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung zum Arbeitsblatt hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Definiere einen Zellbereich für die bedingte Formatierung
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Eine bedingte Formatierungsregel für Datenleisten hinzufügen
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Greife auf das DataBar-Objekt zu
            DataBar dataBar = fc.DataBar;

            // Setze die Farbe der Datenleiste
            dataBar.Color = Color.Blue;

            // Setze die minimale und maximale Länge der Datenleiste
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Setze den Randtyp der Datenleiste
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Setze die Randfarbe der Datenleiste
            dataBar.BarBorder.Color = Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


