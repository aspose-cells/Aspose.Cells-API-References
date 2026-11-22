---
title: "LowCodeSaveOptions.OutputStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptions. تحصل وتعيّن الـ Stream لكتابة البيانات المولدة إليه. عند تعيين هذه الخاصية بقيمة غير فارغة سيتم تجاهل OutputFile"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

تحصل وتعيّن الـ Stream لكتابة البيانات المولدة إليه. عند تعيين هذه الخاصية بقيمة غير فارغة، سيتم تجاهل [`OutputFile`](../outputfile/).

```csharp
public Stream OutputStream { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // إنشاء كائن LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // إنشاء تدفق ذاكرة للتوضيح
                using (MemoryStream stream = new MemoryStream())
                {
                    // تعيين خاصية OutputStream
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // حفظ باستخدام الخيارات (سيتم الكتابة إلى تدفق الذاكرة الخاص بنا)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // تحقق من أنه تم كتابة البيانات إلى التدفق
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // إنشاء مصنف جديد من التدفق للتحقق من المحتوى
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


