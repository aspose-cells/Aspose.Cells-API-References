---
title: "IconSet.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconSet. Получить или установить тип набора значков для отображения. При установке типа будет автоматически проверяться, соответствует ли текущее количество Cfvoss новому типу. Если не соответствует, старые Cfvos будут очищены, и будут добавлены значения Cfvos по умолчанию."
type: docs
url: /ru/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Получить или установить тип набора значков для отображения. При установке типа будет автоматически проверяться, соответствует ли количество текущих Cfvos новому типу. Если не соответствует, старые Cfvos будут удалены, а будут добавлены значения Cfvos по умолчанию.

```csharp
public IconSetType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Продемонстрировать использование свойства Type
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


