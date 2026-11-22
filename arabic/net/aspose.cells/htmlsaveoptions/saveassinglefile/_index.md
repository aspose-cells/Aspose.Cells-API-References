---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم حفظ HTML كملف واحد. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

يشير إلى ما إذا كان سيتم حفظ html كملف واحد. القيمة الافتراضية هي false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### ملاحظات

إذا كان هناك عدة أوراق عمل أو موارد أخرى مطلوبة مثل الصور في المصنف، عادةً ما تحتاج تلك الأوراق والموارد إلى حفظها في ملفات منفصلة. لبعض السيناريوهات، قد يحتاج المستخدم إلى الحصول على ملف ناتج واحد فقط لتسهيل النقل. في هذه الحالة، يمكن للمستخدم تعيين هذه الخاصية إلى true.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // تهيئة خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // حفظ المصنف كملف HTML واحد
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // تحقق من وجود ملف الإخراج
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


