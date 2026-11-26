---
title: "BorderCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BorderCollection. Получает элемент Border по указанному индексу"
type: docs
url: /ru/net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Получает элемент [`Border`](../../border/) по указанному индексу.

```csharp
public Border this[BorderType borderType] { get; }
```

| Параметр | Описание |
| --- | --- |
| borderType | Граница, которую нужно получить. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Получите ячейку и её стиль
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Получите доступ к BorderCollection из стиля
                BorderCollection borders = style.Borders;

                // Отобразите текущее значение свойства Item (операция чтения)
                // Примечание: свойство Item доступно только для чтения и возвращает объект Border
                // Свойству Item требуется параметр BorderType
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Сохранить результат
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


