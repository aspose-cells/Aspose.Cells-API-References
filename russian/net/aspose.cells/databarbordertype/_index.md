---
title: "Перечисление DataBarBorderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DataBarBorderType. Указывает тип границы полосы данных"
type: docs
url: /ru/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Указывает тип границы гистограммы.

```csharp
public enum DataBarBorderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Полоса данных без границы. |
| Solid | `1` | Полоса данных имеет сплошную границу. |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование к рабочему листу
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Определить область ячеек для условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Добавить правило условного форматирования с полосой данных
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Получить доступ к объекту DataBar
            DataBar dataBar = fc.DataBar;

            // Установить цвет полосы данных
            dataBar.Color = Color.Blue;

            // Установить минимальную и максимальную длину полосы данных
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Установить тип границы полосы данных
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Установить цвет границы полосы данных
            dataBar.BarBorder.Color = Color.Red;

            // Сохраните книгу
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


