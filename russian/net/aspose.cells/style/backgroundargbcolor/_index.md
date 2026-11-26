---
title: "Style.BackgroundArgbColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает и задает цвет фона с 32‑битным значением ARGB"
type: docs
url: /ru/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Получает и задает цвет фона в виде 32‑битного значения ARGB.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


