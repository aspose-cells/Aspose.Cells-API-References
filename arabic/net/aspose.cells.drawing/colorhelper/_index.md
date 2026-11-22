---
title: "الفئة ColorHelper"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ColorHelper. توفر وظائف مساعدة حول اللون"
type: docs
url: /ar/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

يوفر وظائف مساعدة حول اللون.

```csharp
public class ColorHelper
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | تحويل OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | تحويل اللون إلى OLE_COLOR |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحويل لون OLE إلى System.Drawing.Color (أخضر)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // تطبيق اللون المحول على خلفية الخلية A1
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // تحويل System.Drawing.Color مرة أخرى إلى لون OLE
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // تحويل نتيجة OLE مرة أخرى إلى Color (التحقق)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // تطبيق اللون المعاد تحويله على خلفية الخلية A2
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // احفظ المصنف المعدل
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


