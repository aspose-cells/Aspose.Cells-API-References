---
title: "BuiltInDocumentPropertyCollection.Category"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يحصل أو يضبط فئة المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

يحصل أو يعيّن فئة المستند.

```csharp
public string Category { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCategoryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            var workbook = new Workbook();
            
            // تعيين خصائص المستند المدمجة
            workbook.BuiltInDocumentProperties.Category = "Financial Report";
            workbook.BuiltInDocumentProperties.ContentStatus = "Final";
            
            // حفظ إلى تدفق الذاكرة
            var stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            
            // حمّل المصنف مرة أخرى من الدفق
            stream.Position = 0;
            var loadedWorkbook = new Workbook(stream);
            
            // اعرض الخصائص
            Console.WriteLine("Category: " + loadedWorkbook.BuiltInDocumentProperties.Category);
            Console.WriteLine("Content Status: " + loadedWorkbook.BuiltInDocumentProperties.ContentStatus);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


