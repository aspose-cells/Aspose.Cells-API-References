---
title: "Validation.GetFormula2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة التحقق. يحصل على القيمة أو التعبير المرتبط بهذا التحقق"
type: docs
url: /ar/net/aspose.cells/validation/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

يحصل على القيمة أو التعبير المرتبط بهذا التحقق.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### قيمة الإرجاع

القيمة أو التعبير المرتبط بهذا التحقق.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تحقق إلى نطاق خلايا
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // إضافة منطقة تحقق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // استدعاء GetFormula2 مع المعلمات (isR1C1: false, isLocal: false)
                string formula2 = validation.GetFormula2(false, false);
                
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // عرض إعدادات التحقق
                Console.WriteLine("Validation Type: " + validation.Type);
                Console.WriteLine("Validation Operator: " + validation.Operator);
                Console.WriteLine("Validation Formula1: " + validation.Formula1);
                Console.WriteLine("Validation Formula2: " + validation.Formula2);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة.

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

القيمة أو التعبير المرتبط بهذا التحقق.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تحقق من البيانات في الخلية A1
            worksheet.Validations.Add();
            Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.Formula2 = "=B1"; // A1-style formula
            validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)

            try
            {
                // الحصول على Formula2 بتنسيق R1C1 للخلية A1
                string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
                Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");

                // إظهار أن الصيغة الأصلية تبقى دون تغيير
                Console.WriteLine($"Original Formula2 (A1 format): {validation.Formula2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2: {ex.Message}");
            }

            workbook.Save("ValidationGetFormula2Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


