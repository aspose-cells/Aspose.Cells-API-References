---
title: "ColorHelper.ToOleColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ColorHelper. تحويل اللون إلى OLE_COLOR"
type: docs
url: /ar/net/aspose.cells.drawing/colorhelper/toolecolor/
---
## ColorHelper.ToOleColor method

تحويل اللون إلى OLE_COLOR

```csharp
public static int ToOleColor(Color color, Workbook workbook)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | كائن Color. |
| المصنف | المصنف |  |

### قيمة الإرجاع

قيمة OLE_COLOR

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ColorHelperMethodToOleColorWithColorWorkbookDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                Color color = Color.Red;

                int oleColor = ColorHelper.ToOleColor(color, workbook);

                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("OLE Color Demonstration");
                
                Style style = workbook.CreateStyle();
                style.ForegroundColor = ColorHelper.FromOleColor(oleColor);
                style.Pattern = BackgroundType.Solid;
                cell.SetStyle(style);

                Console.WriteLine($"Converted OLE Color: {oleColor}");
                Console.WriteLine("Cell A1 background set using converted color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ToOleColorWithColorWorkbookDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../../aspose.cells/workbook/)
* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


