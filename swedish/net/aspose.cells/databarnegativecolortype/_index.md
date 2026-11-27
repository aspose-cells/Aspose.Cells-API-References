---
title: "Enum DataBarNegativeColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBarNegativeColorType‑enum. Anger om samma kant- och fyllningsfärg som positiva datastaplar ska användas"
type: docs
url: /sv/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Anger om samma kant- och fyllningsfärg som positiva datastaplar ska användas.

```csharp
public enum DataBarNegativeColorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Color | `0` | Använd färgen som anges i dialogrutan Negativt värde och axelinställning eller genom att använda egenskaperna ColorType och BorderColorType i NegativeBarFormat‑objektet. |
| SameAsPositive | `1` | Använd samma färg som positiva datastaplar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Ange egenskaperna för datastapeln
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Ange egenskaperna för negativ stapelformatering
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Spara arbetsboken
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


