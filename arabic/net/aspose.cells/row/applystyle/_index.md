---
title: "Row.ApplyStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. تطبق التنسيقات على صف كامل"
type: docs
url: /ar/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

يطبق التنسيقات على الصف بأكمله.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | كائن النمط الذي سيُطبق. |
| علامة | StyleFlag | العلامات التي تشير إلى خصائص التنسيق المطبقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين محتوى HTML في الخلية الأولى
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // الحصول على الصف الأول ونمطه
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // تعديل خصائص النمط
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // تطبيق النمط مع علامات محددة (سيتم تطبيق التفاف النص فقط)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // ملاءمة تلقائية للعرض
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // احفظ المصنف
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


