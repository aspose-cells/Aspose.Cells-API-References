---
title: "MetadataOptions.Password"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MetadataOptions. تمثل كلمة مرور تشفير ملف Workbook"
type: docs
url: /ar/net/aspose.cells.metadata/metadataoptions/password/
---
## MetadataOptions.Password property

يمثل كلمة مرور تشفير ملف Workbook.

```csharp
public string Password { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class MetadataOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // إنشاء خيارات البيانات الوصفية مع حماية كلمة المرور
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "secure_password123";
            
            // إنشاء دفتر عمل جديد وحفظه أولاً
            Workbook workbook = new Workbook();
            string filePath = "ProtectedMetadata.xlsx";
            workbook.Save(filePath);
            
            // تحميل البيانات الوصفية من الملف المحفوظ
            WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);
            
            // إضافة خاصية مستند مخصصة
            metadata.CustomDocumentProperties.Add("CreatedBy", "MetadataDemo");
            
            // حفظ مع البيانات الوصفية
            metadata.Save(filePath);
        }
    }
}
```

### انظر أيضًا

* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


