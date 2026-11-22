---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. الدليل الذي سيتم حفظ الملفات المرفقة فيه. فقط لحفظ إلى تدفق html"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق html.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // إنشاء دليل مؤقت للتوضيح
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // إنشاء مصنف تجريبي
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // تعيين خيارات حفظ HTML باستخدام AttachedFilesDirectory
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // حفظ المصنف كملف HTML
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // تحقق من إنشاء الملفات المرفقة
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // تنظيف
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


