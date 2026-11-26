---
title: "Style.IsTextWrapped"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задает значение, указывающее, будет ли текст в ячейке перенесён"
type: docs
url: /ru/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Получает или задает значение, указывающее, переносится ли текст внутри ячейки.

```csharp
public bool IsTextWrapped { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Установите длинный текст в ячейку
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Включите перенос текста
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Отрегулируйте высоту строки, чтобы отобразить перенесённый текст
            ws.AutoFitRow(0);
            
            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


