---
title: "التعداد ColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.ColorType. يمثل جميع أنواع الألوان"
type: docs
url: /ar/net/aspose.cells/colortype/
---
## ColorType enumeration

يمثل جميع أنواع الألوان

```csharp
public enum ColorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | لون تلقائي. |
| AutomaticIndex | `1` | إنه لون تلقائي، لكن اللون المعروض يعتمد على إعداد نظام التشغيل. |
| RGB | `2` | لون RGB. |
| IndexedColor | `3` | فهرس اللون في لوحة الألوان. |
| Theme | `4` | لون السمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد للعرض
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض استخدام قيم تعداد ColorType
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // عرض قيم التعداد
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // إنشاء خلية وتعيين قيمتها
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // إنشاء نمط وتطبيقه على الخلية
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // احفظ المصنف
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


