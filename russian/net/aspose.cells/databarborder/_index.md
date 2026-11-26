---
title: "Класс DataBarBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataBarBorder. Представляет границу полос данных, указанных правилом условного форматирования"
type: docs
url: /ru/net/aspose.cells/databarborder/
---
## DataBarBorder class

Представляет границу полос данных, указанных правилом условного форматирования.

```csharp
public class DataBarBorder
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Получает или задает цвет границы полос данных, указанных правилом условного форматирования. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Получает или задает тип границы полос данных, указанных правилом условного форматирования. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Создание новой рабочей книги
            Workbook workbook = new Workbook();
            // Доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление образцовых данных в лист
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Добавление пустого условного форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Определение диапазона ячеек для условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Добавление условия типа DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Доступ к DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Установка свойств DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Доступ к свойствам DataBarBorder и их установка
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Сохранение файла Excel
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


