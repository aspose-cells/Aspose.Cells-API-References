---
title: "PasteOptions.Transpose"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. True, чтобы транспонировать строки и столбцы при вставке диапазона. Значение по умолчанию — False"
type: docs
url: /ru/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True для транспонирования строк и столбцов при вставке диапазона. Значение по умолчанию — False.

```csharp
public bool Transpose { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать стиль источника и применить к горизонтальному диапазону
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Создать параметры вставки с транспонированием
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Копировать с транспонированием в вертикальный диапазон
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Сохраните книгу
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### См. также

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


