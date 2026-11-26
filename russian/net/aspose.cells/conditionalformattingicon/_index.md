---
title: "Класс ConditionalFormattingIcon"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ConditionalFormattingIcon. Представляет пользовательский значок правила условного форматирования."
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Представляет пользовательскую иконку правила условного форматирования.

```csharp
public class ConditionalFormattingIcon
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Получает данные набора значков. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Получает и устанавливает индекс значка в наборе значков. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Получает и устанавливает тип набора значков. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Получает данные изображения с настройкой ячейки. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Получить данные набора значков |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу в рабочей книге
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию условных форматирований
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Добавьте новое условное форматирование в коллекцию
            int index = cformattings.Add();
            
            // Получите доступ к коллекции условий форматирования
            FormatConditionCollection fcs = cformattings[index];
            
            // Определите область ячеек для применения условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Добавьте область ячеек в коллекцию условий форматирования
            fcs.AddArea(ca);
            
            // Добавьте условие для использования наборов значков
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Установите тип набора значков
            fc.IconSet.Type = IconSetType.Arrows3;

            // Настройте отдельные значки внутри набора значков
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Сохраните книгу
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


