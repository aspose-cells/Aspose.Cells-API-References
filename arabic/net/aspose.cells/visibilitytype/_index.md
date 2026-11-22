---
title: "التعداد VisibilityType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.VisibilityType. يمثل حالات رؤية الورقة"
type: docs
url: /ar/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

يمثل حالات إظهار الورقة.

```csharp
public enum VisibilityType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Visible | `0` | يشير إلى أن الورقة مرئية. |
| Hidden | `1` | يشير إلى أن الورقة مخفية، ولكن يمكن للمستخدم إظهارها عبر واجهة المستخدم. |
| VeryHidden | `2` | يشير إلى أن الورقة مخفية ولا يمكن إظهارها في واجهة المستخدم (UI). هذه الحالة متاحة فقط برمجياً. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين اسم ورقة العمل
            worksheet.Name = "DemoSheet";

            // تعيين رؤية ورقة العمل إلى مخفي
            worksheet.VisibilityType = VisibilityType.Hidden;

            // احفظ المصنف
            workbook.Save("VisibilityTypeExample.xlsx");

            // إخراج للإشارة إلى اكتمال العملية
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


