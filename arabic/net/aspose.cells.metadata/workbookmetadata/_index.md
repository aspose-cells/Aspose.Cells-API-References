---
title: "الفئة WorkbookMetadata"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Metadata.WorkbookMetadata فئة. يمثل البيانات الوصفية"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/
---
## WorkbookMetadata class

يمثل بيانات التعريف.

```csharp
public class WorkbookMetadata
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkbookMetadata](workbookmetadata/#constructor)(Stream, MetadataOptions) | إنشاء كائن البيانات الوصفية. |
| [WorkbookMetadata](workbookmetadata/#constructor_1)(string, MetadataOptions) | إنشاء كائن البيانات الوصفية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BuiltInDocumentProperties](../../aspose.cells.metadata/workbookmetadata/builtindocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [CustomDocumentProperties](../../aspose.cells.metadata/workbookmetadata/customdocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [Options](../../aspose.cells.metadata/workbookmetadata/options/) { get; } | يحصل على خيارات البيانات الوصفية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save)(Stream) | احفظ البيانات الوصفية المعدلة إلى التدفق. |
| [Save](../../aspose.cells.metadata/workbookmetadata/save/#save_1)(string) | احفظ البيانات الوصفية المعدلة إلى الملف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using Aspose.Cells.Properties;
    using System;
    using System.IO;

    public class WorkbookMetadataDemo
    {
        public static void WorkbookMetadataExample()
        {
            // إنشاء مثيل MetadataOptions
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

            // إنشاء مثيل WorkbookMetadata مع اسم ملف وخيارات
            WorkbookMetadata meta = new WorkbookMetadata("WorkbookMetadataExample_original.xlsx", options);

            // إضافة خاصية مستند مخصصة
            meta.CustomDocumentProperties.Add("test", "test");

            // احفظ البيانات الوصفية إلى ملف جديد
            meta.Save("WorkbookMetadataExample.xlsx");

            // عرض الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProps = meta.BuiltInDocumentProperties;
            Console.WriteLine("Author: " + builtInProps.Author);
            Console.WriteLine("Title: " + builtInProps.Title);

            // عرض الوصول إلى خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProps = meta.CustomDocumentProperties;
            foreach (DocumentProperty prop in customProps)
            {
                Console.WriteLine("Custom Property - Name: " + prop.Name + ", Value: " + prop.Value);
            }

            // احفظ البيانات الوصفية إلى تدفق
            using (FileStream stream = new FileStream("WorkbookMetadataExample2.xlsx", FileMode.Create, FileAccess.Write))
            {
                meta.Save(stream);
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Metadata](../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../)


