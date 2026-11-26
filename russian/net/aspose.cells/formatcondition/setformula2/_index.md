---
title: "FormatCondition.SetFormula2"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatCondition. Устанавливает значение или выражение, связанное с этим условием форматирования"
type: docs
url: /ru/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Задает значение или выражение, связанное с этим условием формата.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // Добавить условие форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Получить первое условие форматирования
            FormatCondition fc = fcs[0];

            try
            {
                // Вызовите SetFormula2 с параметрами (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // Отобразить результат
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Примените некоторый стиль, чтобы эффект был виден
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### См. также

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


