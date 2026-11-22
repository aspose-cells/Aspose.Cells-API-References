---
title: "BuiltInDocumentPropertyCollection.ContentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يحصل أو يضبط نوع محتوى المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

يحصل أو يعيّن نوع محتوى المستند.

```csharp
public string ContentType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyContentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // قم بتعيين خاصية ContentType
            workbook.BuiltInDocumentProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";

            // اعرض خاصية ContentType
            Console.WriteLine("ContentType: " + workbook.BuiltInDocumentProperties.ContentType);

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


