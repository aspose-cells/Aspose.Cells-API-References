---
title: "Класс IconSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.IconSet. Описывает правило условного форматирования IconSet. Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями"
type: docs
url: /ru/net/aspose.cells/iconset/
---
## IconSet class

Описывает правило условного форматирования IconSet. Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями.

```csharp
public class IconSet
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Получить [`ConditionalFormattingIcon`](../conditionalformattingicon/) из коллекции |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Получить экземпляр CFValueObjects. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Указывает, является ли набор значков пользовательским. Значение по умолчанию — false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Получить или установить флаг, указывающий, следует ли изменить порядок значков в этом наборе значков на обратный. Значение по умолчанию — false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Получить или установить флаг, указывающий, следует ли отображать значения ячеек, к которым применён этот набор значков. Значение по умолчанию — true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Получить или установить тип набора значков для отображения. При установке типа будет автоматически проверяться, соответствует ли количество текущих Cfvos новому типу. Если не соответствует, старые Cfvos будут удалены, а будут добавлены значения Cfvos по умолчанию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Добавляет условие
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Получить набор значков
            IconSet iconSet = cond.IconSet;

            // Установить тип значка
            iconSet.Type = IconSetType.Arrows3;

            // Установить дополнительные свойства
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Задать значения ячеек
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Сохранение файла Excel
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


