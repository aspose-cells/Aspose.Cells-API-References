---
title: "FormatCondition.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получает или задает стиль условно отформатированных диапазонов ячеек"
type: docs
url: /ru/net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

Получает или задает стиль диапазонов ячеек, условно отформатированных.

```csharp
public Style Style { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStyleDemo
    {
        public static void Run()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(30);
            worksheet.Cells["A2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(90);

            // Добавить условное форматирование
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Установить диапазон
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            // Добавить первое условие (значения от 40 до 80)
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
            fc1.Style.Font.Color = System.Drawing.Color.Black;

            // Добавить второе условие (значения > 80)
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;
            fc2.Style.Font.Color = System.Drawing.Color.White;
            fc2.Style.Font.IsBold = true;

            // Сохраните книгу
            workbook.Save("FormatConditionStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


