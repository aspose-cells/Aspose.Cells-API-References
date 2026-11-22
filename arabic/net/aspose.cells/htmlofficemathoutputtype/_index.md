---
title: "التعداد HtmlOfficeMathOutputType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.HtmlOfficeMathOutputType. يمثل طريقة تصدير OfficeMath إلى HTML"
type: docs
url: /ar/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

يمثل طريقة تصدير OfficeMath إلى HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Image | `0` | يحوّل OfficeMath إلى HTML كصورة محددة بواسطة وسم &lt;img&gt;. |
| MathML | `1` | يحوّل OfficeMath إلى HTML باستخدام MathML. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة OfficeMath إلى الخلية A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين نوع إخراج OfficeMath إلى صورة
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // حفظ بنوع إخراج صورة
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // تغيير نوع الإخراج إلى MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // حفظ بنوع إخراج MathML
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


