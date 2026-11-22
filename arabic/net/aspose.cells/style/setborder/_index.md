---
title: "Style.SetBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تعيّن حدود النمط"
type: docs
url: /ar/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

يضبط حدود النمط.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | BorderType | الحد(ود) التي سيتم تعيينها، يمكن أن تكون مزيجًا من [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | نمط الحد. |
| borderColor | اللون | لون الحد. |

### قيمة الإرجاع

ما إذا تم تغيير إعدادات الحد الحالية.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

يضبط حدود النمط.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderType | BorderType | الحد(ود) التي سيتم تعيينها، يمكن أن تكون مزيجًا من [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | نمط الحد. |
| borderColor | CellsColor | لون الحد. |

### قيمة الإرجاع

ما إذا تم تغيير إعدادات الحد الحالية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // إنشاء نمط
                Style style = workbook.CreateStyle();
                
                // إنشاء كائن CellsColor باستخدام طريقة المصنع المناسبة
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // استدعاء SetBorder مع معلمات BorderType و CellBorderType و CellsColor
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // تطبيق النمط على خلية
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // احفظ المصنف
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


