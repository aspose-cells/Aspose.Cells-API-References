---
title: "FormatCondition.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Textvärdet i en text innehåller villkorsformateringsregel. Giltig endast för typerna containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null."
type: docs
url: /sv/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

Textvärdet i en "text contains"-villkorlig formateringsregel. Giltig endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null.

```csharp
public string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Lägg till textvillkor
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Ange textegenskapen (visar rysk text)
            formatCondition.Text = "вс";

            // Tillämpa formateringsstil
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Tillämpa på cell A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Spara och verifiera
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Se även

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


