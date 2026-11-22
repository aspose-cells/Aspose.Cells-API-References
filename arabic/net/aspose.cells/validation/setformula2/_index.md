---
title: "Validation.SetFormula2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة التحقق. يحدد القيمة أو التعبير المرتبط بهذا التحقق"
type: docs
url: /ar/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

يضبط القيمة أو التعبير المرتبط بهذا التحقق.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| isR1C1 | منطقي | ما إذا كانت الصيغة صيغة R1C1. |
| isLocal | منطقي | ما إذا كانت الصيغة مُنسقة محليًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء قيم المرجع النموذجية
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // إنشاء تحقق من البيانات للخلية C1
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // تكوين معلمات التحقق
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // تعيين صيغ التحقق باستخدام أنواع المعلمات المطلوبة
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


