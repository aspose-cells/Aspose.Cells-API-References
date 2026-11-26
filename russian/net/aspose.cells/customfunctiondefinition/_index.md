---
title: "Класс CustomFunctionDefinition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CustomFunctionDefinition. Определение пользовательской функции для вычислений с пользовательским движком"
type: docs
url: /ru/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

Определение пользовательской функции для вычислений с использованием пользовательского движка.

```csharp
public class CustomFunctionDefinition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Получает индексы параметров заданной пользовательской функции, которые необходимо вычислить в режиме массива. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать новый экземпляр CustomFunctionDefinition
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Создать новый экземпляр FormulaParseOptions и установить CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Добавить лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Определить пользовательскую формулу
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Разобрать пользовательскую формулу с использованием FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Сохраните книгу
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


