---
title: "Класс ColorHelper"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.ColorHelper. Предоставляет вспомогательные функции для работы с цветом"
type: docs
url: /ru/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Предоставляет вспомогательные функции, связанные с цветом.

```csharp
public class ColorHelper
```

## Методы

| Имя | Описание |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Преобразовать OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Преобразовать цвет в OLE_COLOR |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Преобразовать OLE-цвет в System.Drawing.Color (Green)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Применить преобразованный цвет к фону ячейки A1
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // Преобразовать System.Drawing.Color обратно в OLE-цвет
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // Преобразовать результат OLE обратно в Color (verification)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Применить повторно преобразованный цвет к фону ячейки A2
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Сохранить изменённую книгу
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


