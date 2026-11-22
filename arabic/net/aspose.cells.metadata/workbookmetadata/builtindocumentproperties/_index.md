---
title: "WorkbookMetadata.BuiltInDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookMetadata. ترجع مجموعة DocumentProperty التي تمثل جميع خصائص المستند المدمجة في جدول البيانات"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

تُرجع مجموعة [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المدمجة في جدول البيانات.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // حفظ المصنف إلى ملف
                string filePath = "BuiltInDocumentPropertiesDemo.xlsx";
                workbook.Save(filePath);

                // أنشئ خيارات البيانات الوصفية لخصائص المستند
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // تهيئة بيانات دفتر العمل الوصفية
                WorkbookMetadata metadata = new WorkbookMetadata(filePath, options);

                // الوصول إلى خصائص المستند المدمجة (للقراءة فقط)
                var builtInProps = metadata.BuiltInDocumentProperties;

                // عرض بعض خصائص المستند المدمجة
                Console.WriteLine("Built-in Document Properties:");
                Console.WriteLine("Author: " + builtInProps.Author);
                Console.WriteLine("Title: " + builtInProps.Title);
                Console.WriteLine("Subject: " + builtInProps.Subject);
                Console.WriteLine("Created Time: " + builtInProps.CreatedTime);
                Console.WriteLine("Last Saved By: " + builtInProps.LastSavedBy);
                Console.WriteLine("Total Editing Time: " + builtInProps.TotalEditingTime);

                // تعديل بعض الخصائص المدمجة (نظرًا لأنها للقراءة والكتابة)
                builtInProps.Author = "Aspose Developer";
                builtInProps.Title = "BuiltIn Properties Demo";
                builtInProps.Subject = "Demonstrating BuiltInDocumentProperties";
                builtInProps.Company = "Aspose";
                builtInProps.Comments = "This demonstrates the BuiltInDocumentProperties API";

                // حفظ تغييرات البيانات الوصفية
                metadata.Save(filePath);

                Console.WriteLine("\nBuilt-in properties have been updated and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


