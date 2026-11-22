---
title: "CustomPropertyCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomPropertyCollection. تضيف معلومات الخاصية المخصصة"
type: docs
url: /ar/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

يضيف معلومات الخاصية المخصصة.

```csharp
public int Add(string name, string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية المخصصة. |
| القيمة | String | قيمة الخاصية المخصصة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomPropertyCollection customProperties = worksheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            foreach (CustomProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


