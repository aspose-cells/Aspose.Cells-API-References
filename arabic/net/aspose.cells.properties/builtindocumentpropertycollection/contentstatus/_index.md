---
title: "BuiltInDocumentPropertyCollection.ContentStatus"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. يحصل على أو يضبط حالة محتوى المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

يحصل أو يعيّن حالة محتوى المستند.

```csharp
public string ContentStatus { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentStatusDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين خصائص المستند المدمجة بما في ذلك ContentStatus
            workbook.BuiltInDocumentProperties.ContentStatus = "Draft";
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";

            // احفظ المصنف
            workbook.Save("DocumentWithContentStatus.xlsx", SaveFormat.Xlsx);

            // تحميل المصنف المحفوظ للتحقق من الخصائص
            Workbook loadedWorkbook = new Workbook("DocumentWithContentStatus.xlsx");
            
            // عرض خاصية ContentStatus
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


