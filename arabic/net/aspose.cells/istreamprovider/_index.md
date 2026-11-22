---
title: "الواجهة IStreamProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الواجهة Aspose.Cells.IStreamProvider. تمثل موفر الدفق المصدر"
type: docs
url: /ar/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

يمثل موفر التدفق المُصدّر.

```csharp
public interface IStreamProvider
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | يغلق الدفق. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | يحصل على الدفق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // تنفيذ طريقة InitStream
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // تنفيذ طريقة CloseStream
        public void CloseStream(StreamProviderOptions options)
        {
            // أغلق الدفق إذا لم يكن فارغًا
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بعض البيانات في ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello World");

            // إنشاء HtmlSaveOptions وتعيين StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // حفظ المصنف بتنسيق HTML
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // تحميل المصنف من تنسيق HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // عرض البيانات المحملة
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


