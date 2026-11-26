---
title: "FormatCondition.SetFormula1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatCondition. Устанавливает значение или выражение, связанное с этим условием форматирования"
type: docs
url: /ru/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Задает значение или выражение, связанное с этим условием формата.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Значение или выражение, связанное с этим условием форматирования. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\"=...\"". |
| isR1C1 | Boolean | Является ли формула формулой R1C1. |
| isLocal | Boolean | Является ли формула локализованной. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить диапазон условного форматирования
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Получить первое условие форматирования
            FormatCondition fc = fcc[0];

            try
            {
                // Вызвать SetFormula1 с параметрами (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Отобразить результат
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


