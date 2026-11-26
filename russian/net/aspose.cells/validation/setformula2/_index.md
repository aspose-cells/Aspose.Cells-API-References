---
title: "Validation.SetFormula2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Устанавливает значение или выражение, связанное с этой проверкой"
type: docs
url: /ru/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

Устанавливает значение или выражение, связанное с этой проверкой.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить образцы справочных значений
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // Создать проверку данных для ячейки C1
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // Настроить параметры проверки
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // Установить формулы проверки, используя требуемые типы параметров
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


