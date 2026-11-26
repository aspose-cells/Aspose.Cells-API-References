---
title: "TableStyleCollection.GetBuiltinTableStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TableStyleCollection. Получает встроенный стиль таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/getbuiltintablestyle/
---
## TableStyleCollection.GetBuiltinTableStyle method

Получает встроенный стиль таблицы

```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | TableStyleType | Тип встроенного стиля таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Получить коллекцию стилей таблицы
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Вызовите GetBuiltinTableStyle с параметром TableStyleType
                TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);

                // Применить встроенный стиль к нашей таблице
                table.TableStyleName = builtinStyle.Name;

                Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


