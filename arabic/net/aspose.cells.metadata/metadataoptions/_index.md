---
title: "الفئة MetadataOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Metadata.MetadataOptions فئة. يمثل خيارات تحميل البيانات الوصفية للملف"
type: docs
url: /ar/net/aspose.cells.metadata/metadataoptions/
---
## MetadataOptions class

يمثل خيارات تحميل بيانات التعريف للملف.

```csharp
public class MetadataOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MetadataOptions](metadataoptions/)(MetadataType) | ينشئ خيارات تحميل البيانات الوصفية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [KeyLength](../../aspose.cells.metadata/metadataoptions/keylength/) { get; set; } | طول المفتاح. |
| [MetadataType](../../aspose.cells.metadata/metadataoptions/metadatatype/) { get; } | يحصل ويضبط نوع البيانات الوصفية التي يتم تحميلها. |
| [Password](../../aspose.cells.metadata/metadataoptions/password/) { get; set; } | يمثل كلمة مرور تشفير ملف Workbook. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsDemo
    {
        public static void MetadataOptionsExample()
        {
            // إنشاء مثيل MetadataOptions بنوع MetadataType محدد
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // تعيين الخصائص
            options.Password = "your_password";
            options.KeyLength = 256;

            // تحميل البيانات الوصفية من دفتر عمل موجود
            WorkbookMetadata metadata = new WorkbookMetadata("MetadataOptionsExample_original.xlsx", options);

            // إضافة خاصية مستند مخصصة
            metadata.CustomDocumentProperties.Add("Author", "John Doe");

            // احفظ تغييرات البيانات الوصفية إلى ملف جديد
            metadata.Save("MetadataOptionsExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


