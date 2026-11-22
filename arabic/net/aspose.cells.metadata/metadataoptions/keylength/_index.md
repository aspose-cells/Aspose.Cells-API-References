---
title: "MetadataOptions.KeyLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MetadataOptions. طول المفتاح"
type: docs
url: /ar/net/aspose.cells.metadata/metadataoptions/keylength/
---
## MetadataOptions.KeyLength property

طول المفتاح.

```csharp
public int KeyLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyKeyLengthDemo
    {
        public static void Run()
        {
            // إنشاء خيارات البيانات الوصفية مع نوع خصائص المستند
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // تعيين خصائص التشفير بما في ذلك KeyLength
            options.Password = "secure_password";
            options.KeyLength = 256; // Using 256-bit encryption
            
            // إنشاء بيانات وصفية لدفتر عمل جديد
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);
            
            // إضافة خاصية مخصصة
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // حفظ مع التشفير
            metadata.Save("encrypted_sample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


