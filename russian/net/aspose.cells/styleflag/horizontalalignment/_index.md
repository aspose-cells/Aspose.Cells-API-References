---
title: "StyleFlag.HorizontalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка горизонтального выравнивания будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Настройка горизонтального выравнивания будет применена.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пример данных в ячейках
            worksheet.Cells["A1"].PutValue("Left Aligned");
            worksheet.Cells["B1"].PutValue("Center Aligned");
            worksheet.Cells["C1"].PutValue("Right Aligned");
            
            // Создайте стили с разными горизонтальными выравниваниями
            Style styleLeft = workbook.CreateStyle();
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            
            Style styleCenter = workbook.CreateStyle();
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            
            Style styleRight = workbook.CreateStyle();
            styleRight.HorizontalAlignment = TextAlignmentType.Right;
            
            // Создайте флаги стилей, чтобы применять только горизонтальное выравнивание
            StyleFlag flag = new StyleFlag();
            flag.HorizontalAlignment = true;
            
            // Примените стили к диапазонам
            Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
            rangeLeft.ApplyStyle(styleLeft, flag);
            
            Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
            rangeCenter.ApplyStyle(styleCenter, flag);
            
            Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
            rangeRight.ApplyStyle(styleRight, flag);
            
            // Сохраните книгу
            workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


