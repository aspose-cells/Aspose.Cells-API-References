---
title: "الفئة CustomProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Properties.CustomProperty class. يمثل خاصية مخصصة تخزن أزواج الاسم والقيمة لبيانات مستخدم عشوائية للورقة."
type: docs
url: /ar/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

يمثل خاصية مخصصة تخزن أزواج الاسم والقيمة لبيانات تعريفية عشوائية يحددها المستخدم لورقة العمل.

```csharp
public class CustomProperty
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | يحصل على قيمة الخاصية المخصصة الثنائية ويضبطها. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | إرجاع أو تعيين اسم الكائن. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) يعيد أو يضبط قيمة الخاصية المخصصة. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | تُعيد أو تُعيّن قيمة الخاصية المخصصة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // الوصول إلى مجموعة CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // إضافة خصائص مخصصة
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // الوصول وعرض الخصائص المخصصة
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // احفظ المصنف
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


