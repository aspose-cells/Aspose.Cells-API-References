---
title: "Cell.GetFormatConditions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على شروط التنسيق التي تُطبق على هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

يحصل على شروط التنسيق التي تُطبق على هذه الخلية.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### قيمة الإرجاع

تُعيد كائن [`FormatConditionCollection`](../../formatconditioncollection/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // أضف بيانات تجريبية
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // إضافة شرط تنسيق إلى الخلية A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // الحصول على شروط التنسيق للخلية A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // إخراج عدد شروط التنسيق
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


