---
title: "تعداد ViewType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ViewType. يمثل نوع العرض لورقة العمل"
type: docs
url: /ar/net/aspose.cells/viewtype/
---
## ViewType enumeration

يمثل نوع العرض لورقة العمل.

```csharp
public enum ViewType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن نوع عرض ورقة العمل إلى PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // احفظ المصنف
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


