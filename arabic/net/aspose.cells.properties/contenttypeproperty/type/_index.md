---
title: "ContentTypeProperty.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ContentTypeProperty. تُرجع وتعيّن نوع الخاصية"
type: docs
url: /ar/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

الحصول على نوع الخاصية وتعيينه.

```csharp
public string Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إضافة خصائص نوع محتوى بأنواع مختلفة
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // الوصول إلى أنواع الخصائص وعرضها
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

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


