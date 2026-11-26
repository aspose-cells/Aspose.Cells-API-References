---
title: "Style.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор Style. Инициализирует новый экземпляр класса Style"
type: docs
url: /ru/net/aspose.cells/style/style/
---
## Style constructor

Инициализирует новый экземпляр класса [`Style`](../).

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Примечания

ПРИМЕЧАНИЕ: Этот конструктор теперь устарел. Вместо него, пожалуйста, используйте метод CellsFactory.CreateStyle(). Это свойство будет удалено через 6 месяцев, начиная с октября 2016 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль, используя конструктор
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


