---
title: "Enum FormatConditionValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FormatConditionValueType enum. Bedingungswerttyp"
type: docs
url: /de/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Bedingungswerttyp.

```csharp
public enum FormatConditionValueType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Formula | `0` | Der minimale / mittlere / maximale Wert für den Farbverlauf wird durch eine Formel bestimmt. |
| Max | `1` | Gibt an, dass der maximale Wert im Bereich als maximaler Wert für den Farbverlauf verwendet werden soll. |
| Min | `2` | Gibt an, dass der minimale Wert im Bereich als minimaler Wert für den Farbverlauf verwendet werden soll. |
| Number | `3` | Gibt an, dass der minimale / mittlere / maximale Wert für den Farbverlauf durch einen konstanten numerischen Wert festgelegt wird. |
| Percent | `4` | Der Wert gibt an, dass ein Prozentsatz zwischen dem minimalen und maximalen Wert im Bereich als minimaler / mittlerer / maximaler Wert für den Farbverlauf verwendet werden soll. |
| Percentile | `5` | Der Wert gibt an, dass ein Perzentilrang im Bereich als minimaler / mittlerer / maximaler Wert für den Farbverlauf verwendet werden soll. |
| AutomaticMax | `6` | Gibt an, dass der automatische maximale Wert im Bereich als automatischer maximaler Wert für den Farbverlauf verwendet werden soll. |
| AutomaticMin | `7` | Gibt an, dass der automatische minimale Wert im Bereich als automatischer minimaler Wert für den Farbverlauf verwendet werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Formatbedingungen hinzufügen
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Icon-Set-Eigenschaften festlegen
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Zellwert festlegen und Formatierung anwenden
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Zugriff auf den Werttyp der Formatbedingung
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Werte aus den Icon-Set-Bedingungen anzeigen
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


