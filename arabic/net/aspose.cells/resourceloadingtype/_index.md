---
title: "تعداد ResourceLoadingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ResourceLoadingType. يمثل طريقة تحميل المورد المرتبط"
type: docs
url: /ar/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

يمثل طريقة تحميل المورد المرتبط.

```csharp
public enum ResourceLoadingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | يقوم بتحميل هذا المورد كالمعتاد. |
| Skip | `1` | يتخطى تحميل هذا المورد. |
| UserProvided | `2` | استخدم التدفق المقدم من المستخدم |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // احفظ دفتر العمل إلى HTML باستخدام موفر تدفق مخصص
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // قدِّم تدفقًا مخصصًا للمورد
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // تخطى تحميل المورد
                options.Stream = Stream.Null;
            }
            else
            {
                // حمِّل المورد كالمعتاد
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // أغلق الدفق إذا لم يكن فارغًا
            options.Stream?.Close();
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


