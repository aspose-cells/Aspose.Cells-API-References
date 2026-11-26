---
title: "DataBar.MinCfvo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получить или установить объект минимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max"
type: docs
url: /ru/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Получить или установить объект минимального значения этого DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Получить коллекцию условного форматирования
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Создать гистограмму с MinCfvo, установленным в тип "Value"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Установить диапазон гистограммы
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Сохраните книгу
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


