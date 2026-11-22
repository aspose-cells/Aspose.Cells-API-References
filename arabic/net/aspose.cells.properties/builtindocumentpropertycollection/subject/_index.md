---
title: "BuiltInDocumentPropertyCollection.Subject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يحصل أو يضبط موضوع المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

يحصل أو يضبط موضوع المستند.

```csharp
public string Subject { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين خصائص المستند المدمجة
            workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
            workbook.BuiltInDocumentProperties.Title = "LiteraTest";

            // احفظ المصنف
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // تحميل المصنف المحفوظ للتحقق من الخصائص
            using (Workbook loadedWorkbook = new Workbook(outputPath))
            {
                string subject = loadedWorkbook.BuiltInDocumentProperties.Subject;
                string title = loadedWorkbook.BuiltInDocumentProperties.Title;

                Console.WriteLine("Subject: " + subject);
                Console.WriteLine("Title: " + title);
            }
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


