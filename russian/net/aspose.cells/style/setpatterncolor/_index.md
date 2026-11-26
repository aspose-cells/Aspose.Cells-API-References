---
title: "Style.SetPatternColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Устанавливает цвет фона"
type: docs
url: /ru/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Устанавливает цвет фона.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шаблон | BackgroundType | Шаблон. |
| color1 | Color | Цвет переднего плана. |
| color2 | Color | Цвет фона. Работает только когда шаблон не равен BackgroundType.None и BackgroundType.Solid. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


