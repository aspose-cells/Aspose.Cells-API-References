---
title: "Enum PaneStateType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.PaneStateType enum. يمثل حالة جزء الأوراق"
type: docs
url: /ar/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

يمثل حالة جزء الورقة.

```csharp
public enum PaneStateType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Frozen | `0` | الأقسام مجمدة، لكنها لم تكن كذلك قبل تجميدها. |
| FrozenSplit | `1` | الأقسام مجمدة وتم تقسيمها قبل تجميدها. |
| Split | `2` | الأقسام مقسمة، لكنها غير مجمدة. |
| Normal | `3` | الأقسام غير مجمدة وغير مقسمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بعض البيانات التجريبية في ورقة العمل
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // تجميد الأقسام عند الخلية B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // تحقق من حالة القسم
            PaneStateType paneState = worksheet.PaneState;

            // إخراج حالة القسم
            Console.WriteLine("Current Pane State: " + paneState);

            // احفظ المصنف
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


