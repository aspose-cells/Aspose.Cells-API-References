---
title: "Validation.SetFormula1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Устанавливает значение или выражение, связанное с этой проверкой"
type: docs
url: /ru/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Устанавливает значение или выражение, связанное с этой проверкой.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Значение или выражение, связанное с этим условием форматирования. |
| isR1C1 | Boolean | Является ли формула формулой R1C1. |
| isLocal | Boolean | Является ли формула локализованной. |

### Примеры

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

            // Подготовьте примерные данные в ячейке B1
            worksheet.Cells["B1"].PutValue(100);

            // Создайте проверку данных для ячейки A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Установите формулу, ссылающуюся на B1, используя обозначение A1 (не R1C1, не локальное)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Сохраните книгу с проверкой данных
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


