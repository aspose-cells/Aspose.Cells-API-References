---
title: "ListColumn.GetDataStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Получает стиль данных в этом столбце таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

Получает стиль данных в этом столбце таблицы.

```csharp
public Style GetDataStyle()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Создайте объект списка (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Получить стиль из первого столбца списка
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Изменить стиль
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Применить измененный стиль обратно к столбцу
            table.ListColumns[0].SetDataStyle(style);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


