---
title: "Row.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Устанавливает стиль этой строки"
type: docs
url: /ru/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Задает стиль этой строки.

```csharp
public void SetStyle(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | стиль, который будет использоваться в качестве стиля по умолчанию для ячеек в этой строке. |

### Примечания

Этот метод только устанавливает указанный стиль в качестве стиля по умолчанию для этой строки, не изменяя настройки стиля для существующих ячеек в этой строке. Чтобы одновременно обновить настройки стиля существующих ячеек до указанного стиля, пожалуйста, используйте [`ApplyStyle`](../applystyle/)

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте и настройте стиль
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Получите первую строку и примените стиль
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Сохраните книгу
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


