---
title: "ChartTextFrame.Characters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartTextFrame. Возвращает объект Characters, представляющий диапазон символов в тексте"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Возвращает объект Characters, представляющий диапазон символов внутри текста.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | Int32 | Индекс начала символа. |
| длина | Int32 | Количество символов. |

### Возвращаемое значение

Объект Characters.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Получить доступ к меткам данных и установить размер шрифта для конкретных символов
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


