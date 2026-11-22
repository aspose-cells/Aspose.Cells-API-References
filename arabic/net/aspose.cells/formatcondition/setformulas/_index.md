---
title: "FormatCondition.SetFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition method. يحدد القيمة أو التعبير المرتبط بهذا الشرط التنسيقي"
type: docs
url: /ar/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

يضبط القيمة أو التعبير المرتبط بشرط التنسيق هذا.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| formula1 | String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا سيتم اعتبارها قيمة عادية (نص, رقم, منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\"=...\"" |
| formula2 | String | القيمة أو التعبير المرتبط بهذا شرط التنسيق. تنسيق الإدخال هو نفسه مع formula1 |
| isR1C1 | منطقي | ما إذا كانت الصيغة صيغة R1C1. |
| isLocal | منطقي | ما إذا كانت الصيغة مُنسقة محليًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


