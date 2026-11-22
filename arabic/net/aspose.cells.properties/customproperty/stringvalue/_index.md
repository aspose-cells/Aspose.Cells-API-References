---
title: "CustomProperty.StringValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomProperty. تُرجع أو تُحدد قيمة الخاصية المخصصة"
type: docs
url: /ar/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

تُعيد أو تُعيّن قيمة الخاصية المخصصة.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية CustomProperty.Value. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2010. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة خاصية مخصصة بقيمة نصية
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // استرجاع الخاصية المخصصة
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // عرض خاصية StringValue (عملية قراءة)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // تعيين قيمة جديدة لخاصية StringValue
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // احفظ المصنف
                workbook.Save("StringValueDemo.xlsx");
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


