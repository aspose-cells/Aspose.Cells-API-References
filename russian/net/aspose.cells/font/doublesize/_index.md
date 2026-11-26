---
title: "Font.DoubleSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает и задает двойной размер шрифта"
type: docs
url: /ru/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Получает и задает двойной размер шрифта.

```csharp
public double DoubleSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


