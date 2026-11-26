---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaParseOptions. Определение для разбора пользовательских функций"
type: docs
url: /ru/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Определение для разбора пользовательских функций.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Примечания

Для некоторых специальных требований, например при вычислении пользовательской функции в пользовательском движке, некоторые её параметры необходимо вычислять в массивном режиме; использование этого свойства позволяет пометить такие параметры как массивные при разборе формулы. В противном случае пользователю потребуется позже обновить эти пользовательские функции с помощью [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/), чтобы получить тот же результат.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать определение пользовательской функции
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // Настроить параметры разбора формулы с пользовательской функцией
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // Установить примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // Использовать пользовательскую функцию в формуле
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // Вычислить книгу, чтобы продемонстрировать обработку пользовательской функции
            workbook.CalculateFormula();

            // Сохранить результат
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


