---
title: "IconSet.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconSet. الحصول على أو تعيين نوع مجموعة الأيقونات للعرض. سيقوم تعيين النوع بالتحقق تلقائيًا إذا كان عدد Cfvoss الحالي يتطابق مع النوع الجديد. إذا لم يتطابق، سيتم تنظيف Cfvos القديمة وإضافة Cfvos الافتراضية."
type: docs
url: /ar/net/aspose.cells/iconset/type/
---
## IconSet.Type property

احصل أو عيّن نوع مجموعة الأيقونات للعرض. سيقوم تعيين النوع بالتحقق تلقائيًا مما إذا كان عدد Cfvos الحالي يتوافق مع النوع الجديد. إذا لم يتوافق، سيتم مسح Cfvos القديمة وإضافة Cfvos الافتراضية.

```csharp
public IconSetType Type { get; set; }
```

### أمثلة

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

            // توضيح استخدام خاصية Type
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


