---
title: "DocumentProperty.Source"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. مصدر المحتوى المرتبط"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

مصدر المحتوى المرتبط.

```csharp
public string Source { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المخصصة
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // أضف خصائص
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // احصل على الخصائص واعرض مصادرها
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // احفظ المصنف
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


