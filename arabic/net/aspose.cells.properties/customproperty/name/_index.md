---
title: "CustomProperty.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomProperty. تُرجع أو تُحدد اسم الكائن"
type: docs
url: /ar/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

إرجاع أو تعيين اسم الكائن.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف خاصية مخصصة مع اسم وقيمة
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // استرجاع الخاصية المخصصة
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // اعرض القيمة الحالية لخاصية Name (عملية قراءة)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // عيّن قيمة جديدة لخاصية Name
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // احفظ المصنف
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


