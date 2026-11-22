---
title: "التعداد PropertyType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Properties.PropertyType. يحدد نوع البيانات لخاصية المستند"
type: docs
url: /ar/net/aspose.cells.properties/propertytype/
---
## PropertyType enumeration

يحدد نوع البيانات لخاصية المستند.

```csharp
public enum PropertyType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Boolean | `0` | الخاصية هي قيمة منطقية. |
| DateTime | `1` | الخاصية هي قيمة تاريخ ووقت. |
| Double | `2` | الخاصية هي رقم عشري. |
| Number | `3` | الخاصية هي رقم صحيح. |
| String | `4` | الخاصية هي قيمة نصية. |
| Blob | `5` | الخاصية هي مصفوفة بايت. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class PropertyTypeDemo
    {
        public static void PropertyTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // تعيين بعض الخصائص المدمجة
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // الوصول إلى خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // إضافة خصائص مخصصة بأنواع مختلفة
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // استرجاع وعرض الخصائص المخصصة
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // احفظ المصنف
            workbook.Save("PropertyTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


