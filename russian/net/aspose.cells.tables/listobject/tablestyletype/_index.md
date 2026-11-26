---
title: "ListObject.TableStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает встроенный стиль таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Получает встроенный стиль таблицы.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Получить коллекцию объектов списка
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Добавить таблицу
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Установить стиль таблицы
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Сохраните книгу
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


