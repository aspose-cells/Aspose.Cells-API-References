---
title: "TableStyleElement.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyleElement. Получает тип элемента"
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Возвращает тип элемента.

```csharp
public TableStyleElementType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Создать таблицу
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Получить стиль таблицы (используя имя стиля вместо создания нового)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Получить доступ к элементам стиля таблицы
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Отобразить текущий тип элемента
            Console.WriteLine("Current Type value: " + element.Type);

            // Примечание: свойство Type только для чтения, поэтому мы не можем установить его
            // element.Type = TableStyleElementType.TotalRow; // Это вызвало бы ошибку компиляции

            // Продемонстрировать, как разные типы элементов влияют на таблицу
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Сохраните книгу
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


