---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تعين اسم مؤلف المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

يحصل أو يعيّن اسم مؤلف المستند.

```csharp
public string Author { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين خاصية المؤلف
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // عرض خاصية المؤلف
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // احفظ المصنف
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


