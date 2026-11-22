---
title: "ConditionalFormattingValue.IsGTE"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingValue. احصل أو عيّن علامة أكبر من أو يساوي. استخدم فقط لمجموعات الأيقونات لتحديد ما إذا كانت قيمة العتبة تستخدم عامل أكبر من أو يساوي. false تشير إلى أن العامل أكبر من يُستخدم بدلاً من أكبر من أو يساوي. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

احصل على أو اضبط علامة أكبر من أو يساوي. استخدمها فقط لمجموعات الأيقونات، تحدد ما إذا كانت قيمة العتبة تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى أن 'greater than' تُستخدم بدلاً من 'greater than or equal to'. القيمة الافتراضية هي true.

```csharp
public bool IsGTE { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // إضافة تنسيق شرطي
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // إنشاء تنسيق مقياس اللون
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // تكوين مقياس لون ثنائي
            fc.ColorScale.Is3ColorScale = false;
            
            // تعيين تنسيق القيمة القصوى (عرض IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // تعيين تنسيق القيمة الدنيا
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // احفظ المصنف
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


