---
title: "BuiltInDocumentPropertyCollection.Title"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. يحصل على أو يضبط عنوان المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/title/
---
## BuiltInDocumentPropertyCollection.Title property

يحصل أو يضبط عنوان المستند.

```csharp
public string Title { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // اضبط خاصية Title
            workbook.BuiltInDocumentProperties.Title = "Sample Document Title";
            
            // اعرض خاصية Title
            Console.WriteLine("Document Title: " + workbook.BuiltInDocumentProperties.Title);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


