---
title: "تعداد CopyFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CopyFormatType enum. يمثل نوع تنسيق النسخ عند إدراج الصفوف"
type: docs
url: /ar/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

يمثل نوع تنسيق النسخ عند إدراج الصفوف.

```csharp
public enum CopyFormatType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| SameAsAbove | `0` | التنسيقات نفس الصف أعلاه. |
| SameAsBelow | `1` | التنسيقات نفس الصف أدناه. |
| Clear | `2` | يمسح التنسيق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // إنشاء InsertOptions وتعيين CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // إدراج صف في الموضع الثاني مع نوع التنسيق المحدد
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // احفظ المصنف
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


