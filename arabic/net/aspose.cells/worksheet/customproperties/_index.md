---
title: "Worksheet.CustomProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ورقة العمل. يحصل على كائن يمثل معلومات المعرف المرتبطة بورقة عمل"
type: docs
url: /ar/net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

يحصل على كائن يمثل معلومات المعرف المرتبطة بورقة العمل.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### ملاحظات

توفر Worksheet.CustomProperties آلية مفضلة لتخزين البيانات العشوائية. إنها تدعم مكونات المستندات من أطراف ثالثة القديمة، وكذلك تلك الحالات التي تحتاج إلى أجزاء ثنائية بشكل صارم.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCustomPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة خصائص مخصصة إلى ورقة العمل
            worksheet.CustomProperties.Add("Property1", "Value1");
            worksheet.CustomProperties.Add("Property2", "12345");
            worksheet.CustomProperties.Add("Property3", DateTime.Now.ToString());
            
            // عرض عدد الخصائص المخصصة
            Console.WriteLine("Custom Properties Count: " + worksheet.CustomProperties.Count);
            
            // الوصول وعرض قيم الخاصية
            foreach (var prop in worksheet.CustomProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // احفظ المصنف
            workbook.Save("WorksheetCustomPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


