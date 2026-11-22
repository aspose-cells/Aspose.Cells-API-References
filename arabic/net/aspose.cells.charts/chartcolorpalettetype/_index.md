---
title: "تعداد ChartColorPaletteType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ChartColorPaletteType تعداد. يعدد جميع لوحات الألوان أحادية اللون المستخدمة في مخطط Excel"
type: docs
url: /ar/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

يسرد جميع لوحات الألوان الأحادية المستخدمة في مخطط Excel.

```csharp
public enum ChartColorPaletteType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | تدرج لون السمة accent1، من الداكن إلى الفاتح. |
| MonochromaticPalette2 | `2` | تدرج لون السمة accent2، من الداكن إلى الفاتح. |
| MonochromaticPalette3 | `3` | تدرج لون السمة accent3، من الداكن إلى الفاتح. |
| MonochromaticPalette4 | `4` | تدرج لون السمة accent4، من الداكن إلى الفاتح. |
| MonochromaticPalette5 | `5` | تدرج لون السمة accent5، من الداكن إلى الفاتح. |
| MonochromaticPalette6 | `6` | تدرج لون السمة accent6، من الداكن إلى الفاتح. |
| MonochromaticPalette7 | `7` | تدرج لون السمة accent7. |
| MonochromaticPalette8 | `8` | تدرج لون السمة accent1، من الفاتح إلى الداكن. |
| MonochromaticPalette9 | `9` | تدرج لون السمة accent2، من الفاتح إلى الداكن. |
| MonochromaticPalette10 | `10` | تدرج لون السمة accent3، من الفاتح إلى الداكن. |
| MonochromaticPalette11 | `11` | تدرج لون السمة accent4، من الفاتح إلى الداكن. |
| MonochromaticPalette12 | `12` | تدرج لون السمة accent5، من الفاتح إلى الداكن. |
| MonochromaticPalette13 | `13` | تدرج لون السمة accent6، من الفاتح إلى الداكن. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف مخططًا تجريبيًا لتوضيح لوحة الألوان
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // أظهر استخدام قيم تعداد ChartColorPaletteType المختلفة
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // عرض قيم التعداد
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // احفظ المصنف
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


