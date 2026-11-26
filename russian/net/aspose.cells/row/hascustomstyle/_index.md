---
title: "Row.HasCustomStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Row. Указывает, имеет ли эта строка пользовательские настройки стиля, отличные от стиля по умолчанию, унаследованного от рабочей книги"
type: docs
url: /ru/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Указывает, имеет ли эта строка пользовательские настройки стиля (отличные от значения по умолчанию, унаследованного от книги).

```csharp
public bool HasCustomStyle { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте и настройте стиль
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Получите доступ к первой строке
            Row row = worksheet.Cells.Rows[0];
            
            // Примените пользовательский стиль к строке
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Проверьте, имеет ли строка пользовательский стиль (должно быть true)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Сохраните книгу
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


