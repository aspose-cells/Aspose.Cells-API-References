---
title: "IconSet.CfIcons"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Obtener theConditionalFormattingIcon de la colección"
type: docs
url: /es/net/aspose.cells/iconset/cficons/
---
## IconSet.CfIcons property

Obtener el[`ConditionalFormattingIcon`](../../conditionalformattingicon/) de la colección

```csharp
public ConditionalFormattingIconCollection CfIcons { get; }
```

### Ejemplos

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

            // Acceder y modificar CfIcons
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

### Ver también

* class [ConditionalFormattingIconCollection](../../conditionalformattingiconcollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


