---
title: "ListObject.UpdateColumnName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Обновляет имена всех столбцов списка в ячейки таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Обновляет имена всех столбцов списка в ячейках таблицы.

```csharp
public void UpdateColumnName()
```

### Примечания

Значения ячеек в строке заголовка таблицы должны совпадать с именем ListColumn; Cell.PutValue не изменяет автоматически имя ListColumn в целях повышения производительности.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Создать объект таблицы/списка
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Заполните таблицу некоторыми данными
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Обновите имена столбцов (будут установлены имена по умолчанию, такие как Column1, Column2 и т.д.)
            listObject.UpdateColumnName();

            // Сохраните книгу
            wb.Save("output.xlsx");

            // Проверьте, что имя столбца было обновлено
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


