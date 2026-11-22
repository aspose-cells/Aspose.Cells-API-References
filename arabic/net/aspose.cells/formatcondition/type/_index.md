---
title: "FormatCondition.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. يحصل أو يضبط ما إذا كان نوع التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

يحصل ويضبط ما إذا كان نوع التنسيق الشرطي.

```csharp
public FormatConditionType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // إنشاء تنسيق شرطي
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // أضف شرط تنسيق بنوع تعبير (معلمات مصححة)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // اضبط النمط للشرط
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // توضيح استخدام خاصية Type
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // احفظ المصنف
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


