---
title: "ContentTypeProperty.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ContentTypeProperty. تُرجع أو تعيّن اسم الكائن"
type: docs
url: /ar/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

إرجاع أو تعيين اسم الكائن.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة خاصية نوع محتوى بالاسم "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // حفظ بصيغة XLS
            workbook.Save("example.xls");
            
            // إعادة تحميل المصنف والتحقق من خاصية Name
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // حفظ بصيغة XLSX
            workbook.Save("example.xlsx");
            
            // إعادة التحميل والتحقق مرة أخرى
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### انظر أيضًا

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


