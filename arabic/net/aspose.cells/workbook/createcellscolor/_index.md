---
title: "Workbook.CreateCellsColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تنشئ كائن CellsColor"
type: docs
url: /ar/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

ينشئ كائن [`CellsColor`](../../cellscolor/)

```csharp
public CellsColor CreateCellsColor()
```

### قيمة الإرجاع

يرجع كائن [`CellsColor`](../../cellscolor/)

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إنشاء نطاق وتعيين حدود بلون مخصص
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // تحقق من نمط الحدود في خلية معينة
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


