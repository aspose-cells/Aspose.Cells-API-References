---
title: "BuiltInDocumentPropertyCollection.Manager"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تعين خاصية المدير"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

يحصل أو يضبط خاصية المدير.

```csharp
public string Manager { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // عيّن خصائص المستند الأساسية بما في ذلك Manager
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
            builtInProperties.Company = "Aspose";

            // احفظ المصنف
            workbook.Save("DocumentPropertiesDemo.xlsx");

            Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


