---
title: "AutoFitterOptions.MaxRowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Получает и задает максимальную высоту строки в единицах Point при автоподгонке строк"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Получает и задает максимальную высоту строки (в единицах Point) при автоматической подгонке строк.

```csharp
public double MaxRowHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyMaxRowHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерные данные и форматирование
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height

            // Создать AutoFitterOptions с параметром MaxRowHeight
            AutoFitterOptions options = new AutoFitterOptions
            {
                MaxRowHeight = 50, // Limit maximum row height to 50 pixels
                OnlyAuto = true
            };

            // Автоподгонка строки с ограничением высоты
            worksheet.AutoFitRows(0, 0, options);

            Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


