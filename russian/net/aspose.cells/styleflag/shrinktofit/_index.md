---
title: "StyleFlag.ShrinkToFit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Параметр Сжатие по размеру будет применён"
type: docs
url: /ru/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Настройка сжатия до размера будет применена.

```csharp
public bool ShrinkToFit { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите примерные данные в ячейку
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Создайте стиль с включённым ShrinkToFit
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Создайте флаг стиля и включите флаг ShrinkToFit
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Примените стиль к диапазону ячеек (явно используя Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Установите ширину столбца, чтобы продемонстрировать сжатие
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Сохраните книгу
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


