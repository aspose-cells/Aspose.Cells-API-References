---
title: "TableStyle.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyle. Получает имя стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Получает имя стиля таблицы.

```csharp
public string Name { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Получить первый стиль таблицы из коллекции
                TableStyle tableStyle = tableStyles[0];

                // Отобразить значение свойства Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Продемонстрировать доступ к свойству только для чтения
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Показать, что мы можем использовать имя для ссылки на стиль
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Сохраните книгу
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


