---
title: "Column.ApplyStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Column. تطبق تنسيقات لعمود كامل"
type: docs
url: /ar/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

يطبق التنسيقات على عمود كامل.

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
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين نص متعدد الأسطر في العمود 2
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // إنشاء نمط مع تمكين التفاف النص
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // تطبيق النمط فقط على خاصية التفاف النص للعمود 2
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


