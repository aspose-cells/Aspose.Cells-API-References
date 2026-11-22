---
title: "Row.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. تعيين النمط لهذا الصف"
type: docs
url: /ar/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

يضبط نمط هذا الصف.

```csharp
public void SetStyle(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | النمط الذي سيُستخدم كنمط افتراضي للخلايا في هذا الصف. |

### ملاحظات

هذه الطريقة تقوم فقط بتعيين النمط المحدد كنمط افتراضي لهذا الصف، دون تغيير إعدادات النمط للخلايا الموجودة في هذا الصف. لتحديث إعدادات النمط للخلايا الموجودة إلى النمط المحدد في الوقت نفسه، يرجى استخدام [`ApplyStyle`](../applystyle/)

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء وتكوين نمط
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // احصل على الصف الأول وطبق النمط
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // احفظ المصنف
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


