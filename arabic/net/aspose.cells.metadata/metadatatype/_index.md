---
title: "التعداد MetadataType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Metadata.MetadataType. يمثل نوع البيانات الوصفية"
type: docs
url: /ar/net/aspose.cells.metadata/metadatatype/
---
## MetadataType enumeration

يمثل نوع بيانات التعريف.

```csharp
[Flags]
public enum MetadataType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Encryption | `1` | يقوم بتشفير الملف. |
| Decryption | `2` | يقوم بفك تشفير الملف. |
| DocumentProperties | `4` | تحميل خصائص الملف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class MetadataTypeDemo
    {
        public static void MetadataTypeExample()
        {
            // تحديد مسار الملف
            string filePath = "MetadataTypeExample_original.xlsx";

            // إنشاء MetadataOptions لخصائص المستند
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // تحميل بيانات التعريف لدفتر العمل
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = metadata.BuiltInDocumentProperties;

            // الوصول إلى خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProperties = metadata.CustomDocumentProperties;

            // عرض بعض الخصائص المدمجة
            Console.WriteLine("Title: " + builtInProperties["Title"]);
            Console.WriteLine("Author: " + builtInProperties["Author"]);
            Console.WriteLine("Company: " + builtInProperties["Company"]);

            // إضافة خاصية مخصصة
            customProperties.Add("MyCustomProperty", "CustomValue");

            // حفظ إلى ملف مختلف
            string newFilePath = "MetadataTypeExample.xlsx";
            metadata.Save(newFilePath);

            Console.WriteLine("Metadata updated and saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


