---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تضبط لغة التحرير الافتراضية"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

يحصل أو يضبط لغة التحرير الافتراضية.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### ملاحظات

قد يعرض/يرسم تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. الافتراضي هو Auto.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // تعيين الخط الافتراضي للدفتر إلى خط يدعم أحرف CJK
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // تعيين النص الياباني الذي سيتطلب التفافًا صحيحًا
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // تكوين تنسيق الخلية - تم الإصلاح باستخدام اسم الخاصية الصحيح
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // إنشاء خيارات تصيير الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // تحويل ورقة العمل إلى صورة
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### انظر أيضًا

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


