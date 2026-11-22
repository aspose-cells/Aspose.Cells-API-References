---
title: "Column.IsCollapsed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. ما إذا كان العمود مطويًا"
type: docs
url: /ar/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

ما إذا كان العمود مطويًا

```csharp
public bool IsCollapsed { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء وتطبيق نمط بسيط على العمود
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // تعيين خصائص العمود بما في ذلك IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // إضافة بعض البيانات لتصوير العمود المطوي
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


