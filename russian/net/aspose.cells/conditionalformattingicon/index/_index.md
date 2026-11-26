---
title: "ConditionalFormattingIcon.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingIcon. Получает и задает индекс значков в наборе значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Получает и устанавливает индекс значка в наборе значков.

```csharp
public int Index { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование набора значков
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // Установить свойства набора значков
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // Отобразите индекс каждого значка
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // Измените и покажите свойство индекса
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### См. также

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


