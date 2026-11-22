---
title: "DocumentProperty.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. تُرجع اسم الخاصية"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

يعيد اسم الخاصية.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // أضف خاصية مخصصة ووضح استخدام Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // الوصول إلى خاصية مدمجة بالاسم
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


