---
title: "FormatCondition.GetFormula1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition method. يحصل على القيمة أو التعبير المرتبط بهذا الشرط التنسيقي"
type: docs
url: /ar/net/aspose.cells/formatcondition/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### قيمة الإرجاع

القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // الحصول على أول شرط تنسيق
            FormatCondition fc = fcc[0];

            try
            {
                // استدعاء GetFormula1 مع معلمات (Boolean, Boolean)
                string formula = fc.GetFormula1(false, false);
                
                Console.WriteLine("Formula1: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // عرض التأثير عن طريق إظهار نطاق التنسيق الشرطي
                Console.WriteLine($"Conditional format applied to range: A1:A3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FormatConditionMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

يحصل على القيمة أو التعبير الخاص بالتنسيق الشرطي للخلية.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

القيمة أو التعبير المرتبط بالتنسيق الشرطي للخلية.

### ملاحظات

يجب أن تكون الخلية المحددة ضمن هذا التنسيق الشرطي، وإلا سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شرط تنسيق
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1, 0));
            int conditionIndex = fcc.AddCondition(FormatConditionType.Expression, OperatorType.None, "=IF(MOD(A1,2)=0,TRUE,FALSE)", null);

            // احصل على الصيغة مع معلمات مختلفة
            FormatCondition condition = fcc[conditionIndex];
            string formula1 = condition.GetFormula1(false, false, 0, 0);
            string formula2 = condition.GetFormula1(false, false, 1, 0);

            Console.WriteLine("Formula for row 0: " + formula1);
            Console.WriteLine("Formula for row 1: " + formula2);
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(int, int) {#getformula1_2}

يحصل على الصيغة الخاصة بالتنسيق الشرطي للخلية.

```csharp
public string GetFormula1(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

الصيغة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula1WithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // الحصول على أول شرط تنسيق
            FormatCondition fc = fcc[0];

            try
            {
                // استدعِ GetFormula1 مع معلمات الصف والعمود المحددة
                string formula = fc.GetFormula1(0, 0);
                
                Console.WriteLine("Formula1 for cell (0,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FormatConditionMethodGetFormula1WithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


