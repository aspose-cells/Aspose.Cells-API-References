---
title: "DocumentProperty.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. تحصل على نوع البيانات للخاصية"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

يحصل على نوع البيانات للخاصية.

```csharp
public PropertyType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المخصصة (غير المدمجة)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // أضف خصائص مخصصة بأنواع مختلفة
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // توضيح استخدام خاصية Type
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // الوصول إلى خاصية محددة وتحقق من نوعها
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


