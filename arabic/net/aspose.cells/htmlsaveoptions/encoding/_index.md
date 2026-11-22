---
title: "HtmlSaveOptions.Encoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. إذا لم يتم تعيينها، استخدم Encoding.UTF8 كنوع الترميز الافتراضي"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

إذا لم يتم تعيينه، استخدم Encoding.UTF8 كنوع الترميز الافتراضي.

```csharp
public Encoding Encoding { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyEncodingDemo
    {
        private class SheetStreamProvider : IStreamProvider
        {
            private readonly MemoryStream _sheet1Stream;
            private readonly MemoryStream _sheet2Stream;
            private int _currentIndex = 0;

            public SheetStreamProvider(MemoryStream sheet1Stream, MemoryStream sheet2Stream)
            {
                _sheet1Stream = sheet1Stream;
                _sheet2Stream = sheet2Stream;
            }

            public void InitStream(StreamProviderOptions options)
            {
                // التهيئة إذا لزم الأمر
            }

            public Stream GetStream(string sheetName)
            {
                return _currentIndex++ == 0 ? _sheet1Stream : _sheet2Stream;
            }

            public void CloseStream(StreamProviderOptions options)
            {
                options.Stream?.Flush();
            }
        }

        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بيانات عينة إلى أوراق العمل
            workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
            workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");

            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // تعيين الترميز إلى UTF8
            saveOptions.Encoding = Encoding.UTF8;

            // إنشاء تدفقات ذاكرة للإخراج
            using (MemoryStream sheet1Stream = new MemoryStream())
            using (MemoryStream sheet2Stream = new MemoryStream())
            {
                // إنشاء موفر تدفق للتعامل مع عدة أوراق
                SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
                saveOptions.StreamProvider = streamProvider;

                // حفظ دفتر العمل مع خيارات HTML
                workbook.Save(new MemoryStream(), saveOptions);

                // تحقق من أن المحتوى تم حفظه بترميز UTF8
                string sheet1Content = Encoding.UTF8.GetString(sheet1Stream.ToArray());
                string sheet2Content = Encoding.UTF8.GetString(sheet2Stream.ToArray());

                Console.WriteLine("Sheet1 content contains text: " + 
                    sheet1Content.Contains("Sample content in Sheet1"));
                Console.WriteLine("Sheet2 content contains text: " + 
                    sheet2Content.Contains("Sample content in Sheet2"));
            }
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


