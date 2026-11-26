---
title: "FormatCondition.IconSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatCondition. Получите экземпляр IconSet условного форматирования. Тип по умолчанию IconSetType — TrafficLights31. Действительно только для типа IconSet"
type: docs
url: /ru/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Получить экземпляр "IconSet" условного форматирования. IconSetType экземпляра по умолчанию — TrafficLights31. Действительно только для type = IconSet.

```csharp
public IconSet IconSet { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Добавить условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Установить диапазон ячеек
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Добавить условие и установить тип в IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Получить IconSet и настроить его
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Сохраните книгу
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### См. также

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


