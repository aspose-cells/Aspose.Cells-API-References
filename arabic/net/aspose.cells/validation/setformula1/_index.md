---
title: "Validation.SetFormula1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة التحقق. يحدد القيمة أو التعبير المرتبط بهذا التحقق"
type: docs
url: /ar/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

يضبط القيمة أو التعبير المرتبط بهذا التحقق.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إعداد بيانات عينة في الخلية B1
            worksheet.Cells["B1"].PutValue(100);

            // إنشاء تحقق من البيانات للخلية A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // تعيين الصيغة التي تشير إلى B1 باستخدام تدوين A1 (ليس R1C1، ليس محليًا)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // حفظ المصنف مع التحقق
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


