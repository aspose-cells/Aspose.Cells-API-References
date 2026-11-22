---
title: "ImageSaveOptions.StreamProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageSaveOptions. يحصل أو يعين IStreamProvider لتصدير الكائنات"
type: docs
url: /ar/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

يحصل أو يعيّن IStreamProvider لتصدير الكائنات.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### ملاحظات

إذا تم الحفظ كـ Tiff، يتم تجاهل هذه الخاصية. وإلا، إذا كان يجب حفظ أكثر من صورة، سنكتب الصور الأخرى باستخدام هذه الخاصية. للاستخدام المتقدم، يرجى استخدام [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) أو [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomStreamProvider : IStreamProvider
    {
        private int m_count = 0;

        public void InitStream(StreamProviderOptions options)
        {
            m_count++;
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            return new FileStream(options.DefaultPath + m_count + ".png", FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // التنفيذ عندما لا يتم توفير تدفق
        }

        public void CloseStream(StreamProviderOptions options, Stream stream)
        {
            stream.Dispose();
        }
    }

    public class ImageSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // تعيين خيارات الحفظ باستخدام موفر تدفق مخصص
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // حفظ باستخدام موفر التدفق
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### انظر أيضًا

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


