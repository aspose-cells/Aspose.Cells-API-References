---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DeleteBlankOptions. Указывает, будут ли объекты, связанные с рисунками, такие как изображения, формы, диаграммы..., считаться пустыми. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Указывает, будут ли графические объекты, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию — true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Примечания

При установке этого свойства в false все строки/столбцы, покрытые объектами рисунков, не будут считаться пустыми и не будут удалены.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Добавьте объект рисунка, чтобы протестировать поведение DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Удалить пустые столбцы с DrawingsAsBlank = false (сохраняет рисунки)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### См. также

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


