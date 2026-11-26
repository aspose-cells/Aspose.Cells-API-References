---
title: "FormatCondition.Operator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получает и задает тип оператора условного форматирования"
type: docs
url: /ru/net/aspose.cells/formatcondition/operator/
---
## FormatCondition.Operator property

Получает и задает тип оператора условного формата.

```csharp
public OperatorType Operator { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyOperatorDemo
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
            
            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Создать диапазон ячеек
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 0;
            
            // Добавить условие
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // Установить стиль
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;
            
            // Продемонстрировать использование свойства Operator
            Console.WriteLine("Operator Type: " + fc.Operator);
            if (fc.Operator == OperatorType.Between)
            {
                Console.WriteLine("Condition is set to BETWEEN values");
            }
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [OperatorType](../../operatortype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


