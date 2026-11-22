---
title: "ColorHelper.FromOleColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ColorHelper. تحويل OLE_COLOR"
type: docs
url: /ar/net/aspose.cells.drawing/colorhelper/fromolecolor/
---
## ColorHelper.FromOleColor method

تحويل OLE_COLOR.

```csharp
public static Color FromOleColor(int oleColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oleColor | Int32 | قيمة OLE_COLOR. |

### قيمة الإرجاع

كائن Color.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ColorHelperMethodFromOleColorWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int oleColor = 0x00FF0000; // OLE color for blue in BGR format
            
            try
            {
                Color convertedColor = ColorHelper.FromOleColor(oleColor);
                
                // تطبيق اللون على خلفية الخلية
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Color converted from OLE");
                Style style = cell.GetStyle();
                style.ForegroundColor = convertedColor;
                style.Pattern = BackgroundType.Solid;
                cell.SetStyle(style);
                
                Console.WriteLine($"Converted OLE color {oleColor:X} to RGB: {convertedColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            
            workbook.Save("ColorHelperMethodFromOleColorWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


