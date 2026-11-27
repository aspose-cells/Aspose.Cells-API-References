---
title: "Enum OperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OperatorType enum. Representerar operatortypen för villkorsformat och datavalidering"
type: docs
url: /sv/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Representerar operatortypen för villkorsformat och datavalidering.

```csharp
public enum OperatorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Between | `0` | Representerar Between-operatorn för villkorsformat och datavalidering. |
| Equal | `1` | Representerar Equal-operatorn för villkorsformat och datavalidering. |
| GreaterThan | `2` | Representerar GreaterThan-operatorn för villkorsformat och datavalidering. |
| GreaterOrEqual | `3` | Representerar GreaterOrEqual-operatorn för villkorsformat och datavalidering. |
| LessThan | `4` | Representerar LessThan-operatorn för villkorsformat och datavalidering. |
| LessOrEqual | `5` | Representerar LessOrEqual-operatorn för villkorsformat och datavalidering. |
| None | `6` | Representerar ingen jämförelse. |
| NotBetween | `7` | Representerar NotBetween-operatorn för villkorsformat och datavalidering. |
| NotEqual | `8` | Representerar NotEqual-operatorn för villkorsformat och datavalidering. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en tom villkorsformatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Ange området för villkorsformatering
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Lägg till ett villkor med OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Lägg till ett annat villkor med OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Spara arbetsboken
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


