---
title: "Column.IsCollapsed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. указывает, свернут ли столбец"
type: docs
url: /ru/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

является ли столбец свернутым

```csharp
public bool IsCollapsed { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте и примените простой стиль к столбцу
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Установите свойства столбца, включая IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Добавьте некоторые данные, чтобы визуализировать свернутый столбец
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


