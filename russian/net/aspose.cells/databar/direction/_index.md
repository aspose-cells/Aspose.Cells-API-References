---
title: "DataBar.Direction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получает или задает направление отображения гистограммы"
type: docs
url: /ru/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Получает или задает направление отображения databar.

```csharp
public TextDirectionType Direction { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные, чтобы продемонстрировать полосы данных
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Добавить условное форматирование полос данных
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Определите область ячеек для условия форматирования
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // Добавьте условие DataBar и получите ссылку
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Отобразите текущее значение Direction
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Измените направление на RightToLeft и продемонстрируйте
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Дополнительная настройка для лучшей визуализации
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Сохраните книгу, чтобы показать эффект
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


