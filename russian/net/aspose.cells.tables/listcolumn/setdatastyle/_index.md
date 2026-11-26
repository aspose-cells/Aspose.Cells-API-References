---
title: "ListColumn.SetDataStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Устанавливает стиль данных в этом столбце таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/setdatastyle/
---
## ListColumn.SetDataStyle method

Устанавливает стиль данных в этом столбце таблицы.

```csharp
public void SetDataStyle(Style style)
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetDataStyleWithStyleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Создайте объект списка (таблица)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Получить стиль первого столбца
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Изменить стиль
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Применить измененный стиль к столбцу
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


