---
title: "Enum DataBarBorderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBarBorderType enum. Anger kanttyp för en datastapel"
type: docs
url: /sv/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Anger kanttypen för en datastapel.

```csharp
public enum DataBarBorderType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Datastapeln har ingen kant. |
| Solid | `1` | Datastapeln har en solid kant. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsstyrd formatering i kalkylbladet
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Definiera ett cellområde för den villkorsstyrda formateringen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Lägg till en villkorsstyrd formateringsregel för datastapel
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Åtkomst till DataBar-objektet
            DataBar dataBar = fc.DataBar;

            // Ange färgen på datastapeln
            dataBar.Color = Color.Blue;

            // Ange minsta och största längden på datastapeln
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Ange kanttyp för datastapeln
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Ange kantfärg för datastapeln
            dataBar.BarBorder.Color = Color.Red;

            // Spara arbetsboken
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


