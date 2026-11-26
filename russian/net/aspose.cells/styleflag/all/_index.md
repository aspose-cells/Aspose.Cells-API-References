---
title: "StyleFlag.All"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Все свойства будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Все свойства будут применены.

```csharp
public bool All { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль с сплошным красным фоном
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Создайте флаг стиля со свойством All, установленным в true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Примените стиль к первому столбцу
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Проверьте, что стиль был применён к ячейкам в столбце
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


