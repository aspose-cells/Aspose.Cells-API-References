---
title: "الفئة Hyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Hyperlink. تغلف الكائن الذي يمثل ارتباطًا تشعبيًا"
type: docs
url: /ar/net/aspose.cells/hyperlink/
---
## Hyperlink class

يغلف الكائن الذي يمثل ارتباطًا تشعبيًا.

```csharp
public class Hyperlink
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | يمثل عنوان الارتباط التشعبي. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | يحصل على نطاق الارتباط التشعبي. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | يحصل على نوع الارتباط. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | إرجاع أو تعيين نص تلميح الشاشة للرابط التشعبي المحدد. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | يمثل النص الذي سيُعرض للرابط التشعبي المحدد. القيمة الافتراضية هي عنوان الرابط التشعبي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | يحذف هذا الرابط التشعبي |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى كائن Workbook
            workbook.Worksheets.Add();
            
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي إلى عنوان URL في الخلية "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // الحصول على رابط تشعبي حسب الفهرس
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // تعيين نص العرض لهذا الرابط التشعبي
            hyperlink.TextToDisplay = "Aspose";
            
            // تعيين نص تلميح الشاشة للرابط التشعبي
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // حفظ ملف Excel
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


