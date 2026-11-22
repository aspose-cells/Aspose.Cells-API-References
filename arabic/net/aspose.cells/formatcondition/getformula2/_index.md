---
title: "FormatCondition.GetFormula2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "FormatCondition method. يحصل على القيمة أو التعبير المرتبط بهذا الشرط التنسيقي"
type: docs
url: /ar/net/aspose.cells/formatcondition/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodGetFormula2WithBooleanBooleanDemo
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

            // إضافة شرط تنسيق
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            
            // تعيين Formula2
            fc.Formula2 = "30";

            try
            {
                // استدعاء GetFormula2 مع معلمات (Boolean, Boolean)
                string formula2 = fc.GetFormula2(false, false);
                
                // اعرض النتيجة
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

يحصل على القيمة أو التعبير الخاص بالتنسيق الشرطي للخلية.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo
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
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "=A3");
            FormatCondition fc = fcs[conditionIndex];

            try
            {
                // استدعاء GetFormula2 مع معلمات محددة (isR1C1, isLocal, row, column)
                string formula = fc.GetFormula2(false, false, 0, 0);
                
                Console.WriteLine("Formula2 retrieved successfully: " + formula);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FormatConditionMethodGetFormula2WithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(int, int) {#getformula2_2}

يحصل على الصيغة الخاصة بالتنسيق الشرطي للخلية.

```csharp
public string GetFormula2(int row, int column)
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

    public class FormatConditionMethodGetFormula2WithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 1;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "A1", "B3");

            // الحصول على أول شرط تنسيق
            FormatCondition fc = fcc[0];

            try
            {
                // استدعاء GetFormula2 مع معلمات الصف والعمود المحددة
                string formula = fc.GetFormula2(1, 0); // Row 1, Column 0 (A2)
                
                Console.WriteLine("Formula2 for cell (1,0): " + formula);
                Console.WriteLine("Method executed successfully with parameters (Int32, Int32)");

                // تطبيق النمط لتصوير التنسيق الشرطي
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("FormatConditionMethodGetFormula2WithInt32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


