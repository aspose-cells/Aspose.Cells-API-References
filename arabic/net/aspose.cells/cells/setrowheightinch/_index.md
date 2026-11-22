---
title: "Cells.SetRowHeightInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تضبط ارتفاع الصف بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

يضبط ارتفاع الصف بوحدة البوصة.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| بوصات | Double | عدد البوصات. يجب أن يكون بين 0 و 409.5/72. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين النمط الافتراضي
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // تعيين ارتفاعات الصفوف بالبوصة
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // احفظ المصنف
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


