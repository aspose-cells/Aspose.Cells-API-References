---
title: "Validation.SetFormula1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama yöntemi. Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar"
type: docs
url: /tr/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Bu biçim koşulu ile ilişkili değer veya ifade. |
| isR1C1 | Boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | Boolean | Formülün yerel biçimlendirilip biçimlendirilmediği. |

### Örnekler

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

            // B1 hücresinde örnek veri hazırlayın
            worksheet.Cells["B1"].PutValue(100);

            // A1 hücresi için veri doğrulaması oluşturun
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // B1'e referans veren formülü A1 gösterimiyle ayarlayın (R1C1 olmayan, yerel olmayan)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Doğrulama ile çalışma kitabını kaydedin
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


