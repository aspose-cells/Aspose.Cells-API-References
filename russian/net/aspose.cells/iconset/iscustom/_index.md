---
title: "IconSet.IsCustom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconSet. Указывает, является ли набор значков пользовательским. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

Указывает, является ли набор значков пользовательским. Значение по умолчанию — false.

```csharp
public bool IsCustom { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Добавить условное форматирование с пользовательским набором значков
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Установить диапазон для условного форматирования
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Добавить условие набора значков
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Установить тип набора значков (используя корректный IconSetType)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // Проверить свойство IsCustom (только для чтения)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


