---
title: "ListObject.Resize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Изменить диапазон объекта списка"
type: docs
url: /ru/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Изменить размер диапазона объекта списка.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Индекс начальной строки нового диапазона. |
| startColumn | Int32 | Индекс начального столбца нового диапазона. |
| endRow | Int32 | Индекс конечной строки нового диапазона. |
| endColumn | Int32 | Индекс конечного столбца нового диапазона. |
| hasHeaders | Boolean | Имеет ли эта таблица заголовки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // Изменить размер объекта списка
            listObj.Resize(0, 0, 9, 1, true);

            // Сохраните книгу
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


