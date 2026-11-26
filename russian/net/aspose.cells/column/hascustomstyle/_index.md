---
title: "Column.HasCustomStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Указывает, имеет ли этот столбец пользовательские настройки стиля, отличные от стиля по умолчанию, унаследованного из рабочей книги"
type: docs
url: /ru/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Указывает, имеет ли этот столбец пользовательские настройки стиля (отличные от настроек по умолчанию, унаследованных из книги).

```csharp
public bool HasCustomStyle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к первой колонке
            Column column = worksheet.Cells.Columns[0];

            // Отобразить начальное значение HasCustomState
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Изменить стиль столбца, чтобы продемонстрировать изменение HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Отобразить обновлённое значение HasCustomStyle
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Создать другой столбец с стилем по умолчанию для сравнения
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Сохраните книгу
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


