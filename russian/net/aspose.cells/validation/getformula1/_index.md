---
title: "Validation.GetFormula1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Validation. Получает значение или выражение, связанное с этой проверкой"
type: docs
url: /ru/net/aspose.cells/validation/getformula1/
---
## GetFormula1(bool, bool) {#getformula1}

Получает значение или выражение, связанное с этой проверкой.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте проверку к первой ячейке
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Примените проверку к ячейке A1
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            try
            {
                // Вызовите GetFormula1 с параметрами (false, false), чтобы получить формулу в обозначении A1
                string formula1 = validation.GetFormula1(false, false);
                
                Console.WriteLine("Formula1 in A1 notation: " + formula1);
                
                // Вызовите GetFormula1 с параметрами (true, false), чтобы получить формулу в обозначении R1C1
                string formula1R1C1 = validation.GetFormula1(true, false);
                
                Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetFormula1(bool, bool, int, int) {#getformula1_1}

Получает значение или выражение, связанное с этой проверкой для конкретной ячейки.

```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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

    public class ValidationMethodGetFormula1WithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте проверку в ячейке B5 (строка 4, столбец 1)
            CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
            int validationIndex = worksheet.Validations.Add(area); // Get validation index
            Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
            validation.Type = ValidationType.Custom;
            validation.Formula1 = "=A5"; // Relative reference to cell A5

            try
            {
                // Вызовите GetFormula1 с форматом R1C1 для ячейки B5
                string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
                Console.WriteLine($"R1C1 Formula: {formulaR1C1}");

                // Вызовите GetFormula1 с форматом A1 для ячейки B5
                string formulaA1 = validation.GetFormula1(false, false, 4, 1);
                Console.WriteLine($"A1 Formula: {formulaA1}");

                workbook.Save("ValidationGetFormula1Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


