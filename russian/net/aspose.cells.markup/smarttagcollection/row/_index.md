---
title: "SmartTagCollection.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagCollection. Возвращает строку смарт‑тегов ячейки"
type: docs
url: /ru/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Получает строку смарт‑тегов ячейки.

```csharp
public int Row { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить умный тег в ячейку A1 (строка 0, столбец 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Получить SmartTagCollection для ячейки A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Отобразить строку ячейки, содержащей эти смарт‑теги
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Примечание: свойство Row только для чтения, поэтому его нельзя установить
            // smartTags.Row = 5; // Это вызовет ошибку компиляции

            // Добавьте ещё один смарт‑тег в ячейку B3 (строка 2, столбец 1), чтобы продемонстрировать другую строку
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Сохраните книгу
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


