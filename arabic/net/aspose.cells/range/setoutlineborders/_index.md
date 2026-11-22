---
title: "Range.SetOutlineBorders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تحدد الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحدود واللون"
type: docs
url: /ar/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

يضبط الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحد واللون.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | CellBorderType | نمط الحدود. |
| borderColor | CellsColor | لون الحدود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء كائن CellsColor بلون سمة
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // إنشاء نطاق وتحديد الحدود الخارجية
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // احفظ المصنف
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

يضبط الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحد واللون.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | CellBorderType | نمط الحدود. |
| borderColor | اللون | لون الحدود. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق من الخلايا (A1:D4)
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // ملء النطاق ببعض البيانات لجعل الحدود مرئية
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // استدعاء SetOutlineBorders بنمط حدود متوسط ولون أحمر
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // حفظ المصنف لرؤية التأثير
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

يضبط حدود الخط الخارجي حول نطاق من الخلايا.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyles | CellBorderType[] | أنماط الحدود. |
| borderColors | Color[] | ألوان الحدود. |

### ملاحظات

يجب أن يكون طول كل من borderStyles و borderStyles هو 4. يجب أن يكون ترتيب borderStyles و borderStyles هو أعلى، أسفل، يسار، يمين

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق من الخلايا (B2:D4)
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // تحضير أنماط الحدود والألوان
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // تحديد الحدود الخارجية بأنماط وألوان مختلفة
                range.SetOutlineBorders(borderStyles, borderColors);

                // ملء الخلايا بالبيانات لجعل الحدود مرئية
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // احفظ المصنف
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


