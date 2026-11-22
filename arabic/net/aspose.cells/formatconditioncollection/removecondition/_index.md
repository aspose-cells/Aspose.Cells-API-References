---
title: "FormatConditionCollection.RemoveCondition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. تزيل شرط التنسيق حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

يزيل شرط التنسيق حسب الفهرس.

```csharp
public void RemoveCondition(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس شرط التنسيق الذي سيتم إزالته. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على مجموعة شروط التنسيق
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // إضافة بعض الشروط النموذجية
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // عرض العدد الأولي
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // إزالة الشرط الأول
                formatConditions.RemoveCondition(index1);
                
                // عرض العدد المحدث
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // احفظ المصنف
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


