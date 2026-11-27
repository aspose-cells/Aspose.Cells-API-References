---
title: "Klass ConditionalFormattingIcon"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConditionalFormattingIcon klass. Representerar den anpassade ikonen för en regel för villkorsstyrd formatering"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Representerar den anpassade ikonen för en villkorsstyrd formateringsregel.

```csharp
public class ConditionalFormattingIcon
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Hämtar ikonuppsättningsdata. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Hämtar och anger ikonens index i ikonuppsättningen. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Hämtar och anger ikonuppsättningstypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Hämtar bilddata med cellens inställning. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Hämta ikonuppsättningsdata |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta Conditional Formattings Collection
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Lägg till en ny villkorsstyrd formatering till samlingen
            int index = cformattings.Add();
            
            // Åtkomst till samlingen för formatvillkor
            FormatConditionCollection fcs = cformattings[index];
            
            // Definiera cellområdet för att tillämpa villkorsstyrd formatering
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Lägg till cellområdet i samlingen för formatvillkor
            fcs.AddArea(ca);
            
            // Lägg till ett villkor för att använda ikonsatser
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Ange ikonsatsens typ
            fc.IconSet.Type = IconSetType.Arrows3;

            // Anpassa de enskilda ikonerna i ikonsatsen
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Spara arbetsboken
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


