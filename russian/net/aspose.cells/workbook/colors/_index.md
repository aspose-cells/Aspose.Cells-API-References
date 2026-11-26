---
title: "Workbook.Colors"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает цвета в палитре для электронной таблицы"
type: docs
url: /ru/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Возвращает цвета в палитре для электронной таблицы.

```csharp
public Color[] Colors { get; }
```

### Примечания

Палитра содержит 56 элементов, каждый представлен RGB‑значением.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к палитре цветов по умолчанию
            Color[] colors = workbook.Colors;

            // Изменить некоторые цвета в палитре
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Создайте лист и добавьте некоторые данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Применить изменённые цвета к ячейкам
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Сохраните книгу
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


