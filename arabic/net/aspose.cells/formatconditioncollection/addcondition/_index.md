---
title: "FormatConditionCollection.AddCondition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FormatConditionCollection. تضيف شرط تنسيق"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

يضيف شرط تنسيق.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | FormatConditionType | نوع شرط التنسيق. |
| operatorType | OperatorType | نوع المشغل |
| formula1 | String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\"=...\"". |
| formula2 | String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. تنسيق الإدخال هو نفسه كما في formula1 |

### قيمة الإرجاع

فهرس كائن شرط التنسيق؛

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

أضف شرط تنسيق.

```csharp
public int AddCondition(FormatConditionType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | FormatConditionType | نوع شرط التنسيق. |

### قيمة الإرجاع

فهرس كائن شرط التنسيق؛

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شروط تنسيق
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // إضافة نطاق
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // إضافة شروط (يعيد فهرسًا من نوع int)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


