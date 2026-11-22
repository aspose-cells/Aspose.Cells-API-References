---
title: "ContentTypeProperty.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ContentTypeProperty. تُرجع أو تعيّن قيمة خاصية نوع المحتوى"
type: docs
url: /ar/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

إرجاع أو تعيين قيمة خاصية نوع المحتوى.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إضافة خاصية نوع محتوى
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // الوصول إلى قيمة الخاصية وتعديلها
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
            // احفظ المصنف
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


