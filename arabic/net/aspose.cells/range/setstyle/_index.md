---
title: "Range.SetStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تطبيق نمط الخلية"
type: docs
url: /ar/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

تطبيق نمط الخلية.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | نمط الخلية. |
| explicitFlag | منطقي | صحيح، فقط استبدال التنسيق الذي تم تعيينه صراحةً. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

يضبط نمط النطاق.

```csharp
public void SetStyle(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | كائن Style. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // تطبيق النمط على خلية
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // أنشئ نطاقًا وطبق النمط نفسه
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // احفظ المصنف
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


