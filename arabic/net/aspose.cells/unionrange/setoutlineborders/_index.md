---
title: "UnionRange.SetOutlineBorders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تضبط حدود الخط الخارجي حول نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/unionrange/setoutlineborders/
---
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_1}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeAColorArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Additional Data");

            // أنشئ نطاقًا وحوله إلى UnionRange
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            UnionRange unionRange = worksheet.Cells.CreateRange(range.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range });

            try
            {
                // حدد أنماط الحدود وألوانها لجميع الحدود الأربعة
                CellBorderType[] borderStyles = new CellBorderType[]
                {
                    CellBorderType.Thin,    // Top border
                    CellBorderType.Medium,  // Right border
                    CellBorderType.Thick,   // Bottom border
                    CellBorderType.Double   // Left border
                };

                Color[] borderColors = new Color[]
                {
                    Color.Red,     // Top border color
                    Color.Blue,    // Right border color
                    Color.Green,   // Bottom border color
                    Color.Orange   // Left border color
                };

                // استدعِ SetOutlineBorders مع المصفوفات
                unionRange.SetOutlineBorders(borderStyles, borderColors);

                Console.WriteLine("SetOutlineBorders method called successfully with CellBorderType[] and Color[] parameters");
                Console.WriteLine($"Applied borders to range: {unionRange.RefersTo}");

                // احفظ المصنف
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders}

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
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test";
            worksheet.Cells["A2"].Value = "More Data";
            worksheet.Cells["B2"].Value = "Example";

            try
            {
                // إنشاء UnionRange يغطي A1:B2
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // حدد حدود الخط الخارجي بنوع حد ولون محددين
                unionRange.SetOutlineBorders(CellBorderType.Medium, Color.Blue);

                Console.WriteLine("SetOutlineBorders method called successfully");
                Console.WriteLine($"Border applied to range: {unionRange.RefersTo}");

                // احفظ المصنف
                workbook.Save("SetOutlineBordersDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOutlineBorders: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellBorderType](../../cellbordertype/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


