---
title: "ConditionalFormattingIconCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingIconCollection. تحصل على عنصر ConditionalFormattingIcon عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

يحصل على عنصر ConditionalFormattingIcon في الفهرس المحدد.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;
            int index = cformattings.Add();
            FormatConditionCollection fcs = cformattings[index];

            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 });
            fcs.AddArea(new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 });

            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // عرض استخدام خاصية Item
            ConditionalFormattingIcon icon = cond.IconSet.CfIcons[0];
            icon.Type = IconSetType.Arrows3;
            icon.Index = 0;

            workbook.Save("ConditionalFormattingIconCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


