---
title: "CustomPropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomPropertyCollection. تحصل على الخاصية المخصصة حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

تحصل على الخاصية المخصصة حسب الفهرس المحدد.

```csharp
public CustomProperty this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

الخاصية المخصصة

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            CustomPropertyCollection customProperties = sheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("DateCreated", DateTime.Now.ToString("yyyy-MM-dd"));
            
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Property {i}: {property.Name} = {property.Value}");
            }
            
            workbook.Save("CustomPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

تحصل على الخاصية المخصصة حسب اسم الخاصية.

```csharp
public CustomProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية. |

### قيمة الإرجاع

الخاصية المخصصة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة خصائص مخصصة
            worksheet.CustomProperties.Add("COR_Report", "Quarterly Report");
            worksheet.CustomProperties.Add("COR_ResultSet", "Sales Data");
            
            // الوصول إلى الخصائص المخصصة وعرضها باستخدام خاصية Item
            Console.WriteLine("COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
            Console.WriteLine("COR_ResultSet: " + worksheet.CustomProperties["COR_ResultSet"].Value);
            
            // تعديل خاصية مخصصة باستخدام خاصية Item
            worksheet.CustomProperties["COR_Report"].Value = "Annual Report";
            Console.WriteLine("Updated COR_Report: " + worksheet.CustomProperties["COR_Report"].Value);
        }
    }
}
```

### انظر أيضًا

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


