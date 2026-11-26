---
title: "Validation.GetFormula2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Получает значение или выражение, связанное с этой проверкой"
type: docs
url: /ru/net/aspose.cells/validation/getformula2/
---
## GetFormula2(bool, bool) {#getformula2}

Получает значение или выражение, связанное с этой проверкой.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Возвращаемое значение

Значение или выражение, связанное с этой проверкой.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodGetFormula2WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить проверку к диапазону ячеек
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Добавить область проверки
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Вызвать GetFormula2 с параметрами (isR1C1: false, isLocal: false)
                string formula2 = validation.GetFormula2(false, false);
                
                Console.WriteLine("Formula2: " + formula2);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
                
                // Отобразить настройки проверки
                Console.WriteLine("Validation Type: " + validation.Type);
                Console.WriteLine("Validation Operator: " + validation.Operator);
                Console.WriteLine("Validation Formula1: " + validation.Formula1);
                Console.WriteLine("Validation Formula2: " + validation.Formula2);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula2(bool, bool, int, int) {#getformula2_1}

Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.

```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Значение или выражение, связанное с этой проверкой.

### Примеры

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

            // Создать проверку данных в ячейке A1
            worksheet.Validations.Add();
            Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.Formula2 = "=B1"; // A1-style formula
            validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)

            try
            {
                // Получить Formula2 в формате R1C1 для ячейки A1
                string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
                Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");

                // Показать, что исходная формула остается неизменной
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

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


