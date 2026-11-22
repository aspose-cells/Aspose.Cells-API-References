---
title: "التعداد HtmlLayoutMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Rendering.HtmlLayoutMode. يمثل وضع التخطيط لعرض HTML"
type: docs
url: /ar/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

يمثل وضع التخطيط لعرض HTML.

```csharp
public enum HtmlLayoutMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Normal | `0` | يعرض المحتوى مثل MS Excel. |
| Print | `1` | يعرض المحتوى في وضع تخطيط الطباعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بعض البيانات النموذجية إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // إنشاء HtmlSaveOptions وتعيين وضع التخطيط إلى Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // حفظ المصنف بوضع التخطيط العادي
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // تغيير وضع التخطيط إلى Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // حفظ المصنف بوضع تخطيط الطباعة
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // عرض قيم التعداد
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


