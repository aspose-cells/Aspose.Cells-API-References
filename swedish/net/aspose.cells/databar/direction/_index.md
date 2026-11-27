---
title: "DataBar.Direction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar property. Hämtar eller anger riktningen som datastapeln visas i"
type: docs
url: /sv/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Hämtar eller anger riktningen som databar visas i.

```csharp
public TextDirectionType Direction { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera datastaplar
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Lägg till villkorlig formatering för datastaplar
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Definiera cellområdet för formatvillkoret
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // Lägg till DataBar-villkoret och hämta referensen
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Visa aktuellt Direction-värde
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Ändra riktning till RightToLeft och demonstrera
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Ytterligare konfiguration för bättre visualisering
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Spara arbetsboken för att visa effekten
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


