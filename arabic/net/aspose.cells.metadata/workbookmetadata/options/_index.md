---
title: "WorkbookMetadata.Options"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookMetadata. تحصل على خيارات البيانات الوصفية"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

يحصل على خيارات البيانات الوصفية.

```csharp
public MetadataOptions Options { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyOptionsDemo
    {
        public static void Run()
        {
            // أنشئ خيارات البيانات الوصفية لخصائص المستند
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // إنشاء نسخة جديدة من بيانات وصفية لدفتر العمل مع الخيارات
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // عرض قيم الخيارات الحالية
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // الوصول إلى خصائص المستند المدمجة
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // إضافة خصائص مستند مخصصة
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // حفظ تغييرات البيانات الوصفية
            metadata.Save("output.xlsx");

            // إنشاء خيارات جديدة للتشفير
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


