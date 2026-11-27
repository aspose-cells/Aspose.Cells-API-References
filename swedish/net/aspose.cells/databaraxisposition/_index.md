---
title: "Enum DataBarAxisPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DataBarAxisPosition-enum. Anger axelpositionen för ett cellintervall med villkorsstyrd formatering som datastaplar"
type: docs
url: /sv/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Anger axelpositionen för ett cellområde med villkorsstyrd formatering som datastaplar.

```csharp
public enum DataBarAxisPosition
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Visa axeln på en variabel position baserat på förhållandet mellan det minsta negativa värdet och det största positiva värdet i intervallet. Positiva värden visas i en vänster‑till‑höger riktning. Negativa värden visas i en höger‑till‑vänster riktning. När alla värden är positiva eller alla värden är negativa visas ingen axel. |
| Midpoint | `1` | Visa axeln i cellens mittpunkt oavsett vilka värden som finns i intervallet. Positiva värden visas i en vänster‑till‑höger riktning. Negativa värden visas i en höger‑till‑vänster riktning. |
| None | `2` | Ingen axel visas, och både positiva och negativa värden visas i en vänster‑till‑höger riktning. |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägger till en regel för villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Ställer in intervallet för villkorsstyrd formatering
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Lägger till ett villkor för datastaplar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Ställer in egenskaper för datastapeln
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
            
            // Sätter cellvärden
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Sparar Excel-filen
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


