---
title: "IconSet.CfIcons"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet‑Eigenschaft. Ruft theConditionalFormattingIcon aus der Sammlung ab"
type: docs
url: /de/net/aspose.cells/iconset/cficons/
---
## IconSet.CfIcons property

Rufen Sie das[`ConditionalFormattingIcon`](../../conditionalformattingicon/) aus der Sammlung ab

```csharp
public ConditionalFormattingIconCollection CfIcons { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyCfIconsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;
            int index = cformattings.Add();
            FormatConditionCollection fcs = cformattings[index];

            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 2 });

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Zugreifen und CfIcons ändern
            ConditionalFormattingIcon icon1 = cond.IconSet.CfIcons[0];
            icon1.Type = IconSetType.Arrows3;
            icon1.Index = 0;

            ConditionalFormattingIcon icon2 = cond.IconSet.CfIcons[1];
            icon2.Type = IconSetType.ArrowsGray3;
            icon2.Index = 1;

            ConditionalFormattingIcon icon3 = cond.IconSet.CfIcons[2];
            icon3.Type = IconSetType.Boxes5;
            icon3.Index = 2;

            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingIconCollection](../../conditionalformattingiconcollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


