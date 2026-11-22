---
title: "BuiltInDocumentPropertyCollection.Words"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يمثل تقديرًا لعدد الكلمات في المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/words/
---
## BuiltInDocumentPropertyCollection.Words property

يمثل تقديرًا لعدد الكلمات في المستند.

```csharp
public int Words { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyWordsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // قم بتعيين خاصية Words
            builtInProperties.Words = 250;

            // أضف بعض المحتوى إلى ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample document");
            worksheet.Cells["A2"].PutValue("Demonstrating the Words property");
            worksheet.Cells["A3"].PutValue("Total words will be set to 250");

            // احفظ المصنف
            workbook.Save("DocumentWithWordsProperty.xlsx");

            Console.WriteLine("Document created with Words property set to: " + builtInProperties.Words);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


