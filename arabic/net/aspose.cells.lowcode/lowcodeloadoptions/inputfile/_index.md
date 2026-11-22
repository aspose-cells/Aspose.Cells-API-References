---
title: "LowCodeLoadOptions.InputFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeLoadOptions. تحصل وتعيّن مسار الملف إذا لزم الأمر للقالب"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

يحصل ويضبط ملف (مع المسار إذا لزم) القالب.

```csharp
public string InputFile { get; set; }
```

### ملاحظات

عند تعيين مسار غير فارغ وغير null لهذه الخاصية، سيتم تجاهل القيمة التي تم تعيينها مسبقاً لـ [`InputStream`](../inputstream/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // إنشاء وحفظ ملف قالب تجريبي
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // تهيئة LowCodeLoadOptions وعرض خاصية InputFile
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // تعيين خاصية InputFile لاستخدام القالب الخاص بنا
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // تحميل المصنف باستخدام ملف القالب المحدد
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // تعديل القالب المحمّل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // احفظ المصنف المعدل
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


