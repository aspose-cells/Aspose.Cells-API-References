---
title: "Enum PivotAreaType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotAreaType Enum. Gibt den Typ der Regel an, die verwendet wird, um einen Bereich oder Aspekt der PivotTable zu beschreiben"
type: docs
url: /de/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Gibt den Typ der Regel an, die verwendet wird, um einen Bereich oder Aspekt der PivotTable zu beschreiben.

```csharp
public enum PivotAreaType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Pivot‑Bereich. |
| Normal | `1` | Stellt einen Header oder ein Element dar. |
| Data | `2` | Stellt etwas im Datenbereich dar. |
| All | `3` | Stellt die gesamte PivotTable dar. |
| Origin | `4` | Stellt die leeren Zellen oben links der PivotTable dar (oben rechts für RTL‑Blätter). |
| Button | `5` | Stellt einen Feld‑Button dar. |
| TopRight | `6` | Stellt die leeren Zellen oben rechts der PivotTable dar (oben links für RTL‑Blätter). |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Erstelle eine PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Felder zur PivotTable hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Erstelle einen PivotArea für die PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Gib die PivotArea-Eigenschaften aus
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


