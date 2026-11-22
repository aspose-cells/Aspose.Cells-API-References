---
title: "BorderCollection.SetColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة BorderCollection. يضبط اللون لجميع الحدود في المجموعة"
type: docs
url: /ar/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

يضبط Color لجميع الحدود في المجموعة.

```csharp
public void SetColor(Color color)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | لون الحدود. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط بحدود ملونة
            Style style = workbook.CreateStyle();
            
            // تعيين أنماط خطوط الحدود
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // تعيين لون الحد إلى الأحمر باستخدام طريقة SetColor
            style.Borders.SetColor(Color.Red);

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // ضبط العمود تلقائيًا لتحسين الرؤية
            worksheet.AutoFitColumn(0);

            // احفظ المصنف
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


