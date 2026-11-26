---
title: "Перечисление TextOverflowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.TextOverflowType. Представляет способ вертикального или горизонтального переполнения текста."
type: docs
url: /ru/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Представляет способ вертикального или горизонтального переполнения текста.

```csharp
public enum TextOverflowType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Clip | `0` | Обратите внимание на верхние и нижние границы. Не предоставляйте никаких указаний на наличие невидимого текста. |
| Ellipsis | `1` | Обратите внимание на верхние и нижние границы. Используйте многоточие, чтобы обозначить наличие невидимого текста. Только для вертикального переполнения. |
| Overflow | `2` | Переполняйте текст и игнорируйте верхние и нижние границы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Добавьте текстовое поле к диаграмме.
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Установите свойства текстового поля.
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Установите тип переполнения текста.
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Сохраните книгу
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


