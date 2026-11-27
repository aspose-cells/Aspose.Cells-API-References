---
title: "ConditionalFormattingCollection.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingCollection-metoden. Kopierar villkorlig formatering"
type: docs
url: /sv/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Kopierar villkorlig formatering.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | Den villkorliga formateringen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Skapa en källarbok med villkorlig formatering
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Lägg till exempel på villkorlig formatering till källbladet
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Skapa och tillämpa stil på formatvillkoret
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Tillämpa på ett område
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Kopiera villkorlig formatering från källa till destination
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Spara arbetsboken
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


