---
title: "تعداد FormatConditionValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FormatConditionValueType. نوع قيمة الشرط"
type: docs
url: /ar/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

نوع قيمة الشرط.

```csharp
public enum FormatConditionValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Formula | `0` | يتم تحديد القيمة الدنيا / المتوسطة / العظمى للتدرج بواسطة صيغة. |
| Max | `1` | يشير إلى أن القيمة العظمى في النطاق ستُستخدم كالقيمة العظمى للتدرج. |
| Min | `2` | يشير إلى أن القيمة الدنيا في النطاق ستُستخدم كالقيمة الدنيا للتدرج. |
| Number | `3` | يشير إلى أن القيمة الدنيا / المتوسطة / العظمى للتدرج محددة بقيمة عددية ثابتة. |
| Percent | `4` | تشير القيمة إلى نسبة مئوية بين القيمتين الدنيا والعظمى في النطاق ستُستخدم كالقيمة الدنيا / المتوسطة / العظمى للتدرج. |
| Percentile | `5` | تشير القيمة إلى ترتيب مئوي في النطاق سيُستخدم كالقيمة الدنيا / المتوسطة / العظمى للتدرج. |
| AutomaticMax | `6` | يشير إلى أن القيمة العظمى التلقائية في النطاق ستُستخدم كالقيمة العظمى التلقائية للتدرج. |
| AutomaticMin | `7` | يشير إلى أن القيمة الدنيا التلقائية في النطاق ستُستخدم كالقيمة الدنيا التلقائية للتدرج. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة شروط التنسيق
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // تعيين خصائص مجموعة الأيقونات
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // تعيين قيمة الخلية وتطبيق التنسيق
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // الوصول إلى نوع قيمة شرط التنسيق
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // عرض القيم من شروط مجموعة الأيقونات
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // احفظ المصنف
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


