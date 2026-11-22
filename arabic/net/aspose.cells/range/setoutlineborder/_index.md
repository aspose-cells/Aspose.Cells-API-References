---
title: "Range.SetOutlineBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تُحدد حدًا خارجيًا حول نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

يضبط حدًا خارجيًا حول نطاق من الخلايا.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderEdge | BorderType | حافة الحدود. |
| borderStyle | CellBorderType | نمط الحدود. |
| borderColor | CellsColor | لون الحدود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء كائن CellsColor
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // إنشاء نطاق وتعيين الحد الأيمن
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // إنشاء نطاق آخر وتعيين جميع الحدود
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // احفظ المصنف
            workbook.Save("SetOutlineBorderExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

يضبط حدًا خارجيًا حول نطاق من الخلايا.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderEdge | BorderType | حافة الحدود. |
| borderStyle | CellBorderType | نمط الحدود. |
| borderColor | اللون | لون الحدود. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق من الخلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // تحديد حدود خارجية بأنواع ألوان حدود مختلفة
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // احفظ المصنف
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


