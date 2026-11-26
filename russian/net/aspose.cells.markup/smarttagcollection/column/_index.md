---
title: "SmartTagCollection.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagCollection. Возвращает столбец смарт‑тегов ячейки"
type: docs
url: /ru/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Получает столбец смарт‑тегов ячейки.

```csharp
public int Column { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте смарт‑тег в ячейку C5 (строка 4, столбец 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Получить SmartTagCollection для ячейки C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Отобразить столбец ячейки, содержащей эти смарт‑теги
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Добавьте ещё один смарт‑тег в ячейку E2 (строка 1, столбец 4), чтобы продемонстрировать другой столбец
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Сохраните книгу
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


