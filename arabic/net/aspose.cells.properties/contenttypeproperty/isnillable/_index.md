---
title: "ContentTypeProperty.IsNillable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ContentTypeProperty. تشير إلى ما إذا كانت القيمة يمكن أن تكون فارغة"
type: docs
url: /ar/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

يشير إلى ما إذا كانت القيمة يمكن أن تكون فارغة.

```csharp
public bool IsNillable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إضافة خاصية نوع محتوى
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // الوصول إلى الخاصية وتعيين IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // التحقق وإخراج قيمة IsNillable
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


