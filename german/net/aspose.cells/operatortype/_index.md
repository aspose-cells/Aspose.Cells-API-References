---
title: "Enum OperatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.OperatorType enum. Stellt den Operatortyp der bedingten Formatierung und Datenvalidierung dar."
type: docs
url: /de/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Stellt den Operator-Typ für bedingte Formatierung und Datenvalidierung dar.

```csharp
public enum OperatorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Between | `0` | Stellt den Between-Operator der bedingten Formatierung und Datenvalidierung dar. |
| Equal | `1` | Stellt den Equal-Operator der bedingten Formatierung und Datenvalidierung dar. |
| GreaterThan | `2` | Stellt den GreaterThan-Operator der bedingten Formatierung und Datenvalidierung dar. |
| GreaterOrEqual | `3` | Stellt den GreaterOrEqual-Operator der bedingten Formatierung und Datenvalidierung dar. |
| LessThan | `4` | Stellt den LessThan-Operator der bedingten Formatierung und Datenvalidierung dar. |
| LessOrEqual | `5` | Stellt den LessOrEqual-Operator der bedingten Formatierung und Datenvalidierung dar. |
| None | `6` | Stellt keinen Vergleich dar. |
| NotBetween | `7` | Stellt den NotBetween-Operator der bedingten Formatierung und Datenvalidierung dar. |
| NotEqual | `8` | Stellt den NotEqual-Operator der bedingten Formatierung und Datenvalidierung dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine leere bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Den Bereich der bedingten Formatierung festlegen
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Eine Bedingung mit OperatorType.Between hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Eine weitere Bedingung mit OperatorType.GreaterThan hinzufügen
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Speichere die Arbeitsmappe
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


