---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookMetadata. تُرجع مجموعة DocumentProperty التي تمثل جميع خصائص المستند المخصصة لجدول البيانات"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

تُرجع مجموعة [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) تمثل جميع خصائص المستند المخصصة لجدول البيانات.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // مسارات المصدر والوجهة
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // أنشئ خيارات البيانات الوصفية لخصائص المستند
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // تهيئة بيانات دفتر العمل الوصفية
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // إضافة خاصية مستند مخصصة
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // حفظ دفتر العمل مع البيانات الوصفية
            meta.Save(destPath);
            
            // التحقق من الخاصية المخصصة
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### انظر أيضًا

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


