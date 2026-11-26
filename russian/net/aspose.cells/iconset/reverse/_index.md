---
title: "IconSet.Reverse"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство IconSet. Получить или установить флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Получить или установить флаг, указывающий, следует ли изменить порядок значков в этом наборе значков на обратный. Значение по умолчанию — false.

```csharp
public bool Reverse { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Установить диапазон
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Создать условное форматирование набора значков
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Настроить набор значков
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Продемонстрировать свойство Reverse
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Сохраните книгу
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


