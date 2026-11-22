---
title: "CustomProperty.BinaryValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomProperty. يحصل على القيمة الثنائية للخاصية المخصصة ويضبطها"
type: docs
url: /ar/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

يحصل على قيمة الخاصية المخصصة الثنائية ويضبطها.

```csharp
public byte[] BinaryValue { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف خاصية مخصصة مع قيمة نموذجية
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // استرجاع الخاصية المخصصة
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // اعرض الاسم والقيمة للخاصية المخصصة
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // ملاحظة: الانعكاس لـ CustomProperty لا يتضمن خاصية BinaryValue.
                // القيمة المتاحة القائمة على السلسلة يمكن الوصول إليها عبر الخاصية 'Value'.

                // احفظ دفتر العمل (اختياري)
                workbook.Save("BinaryValueDemo.xlsx");
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


