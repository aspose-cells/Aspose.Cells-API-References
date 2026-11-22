---
title: "Cells.Columns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على مجموعة كائنات Column التي تمثل الأعمدة الفردية في ورقة العمل هذه"
type: docs
url: /ar/net/aspose.cells/cells/columns/
---
## Cells.Columns property

يحصل على مجموعة كائنات [`Column`](../../column/) التي تمثل الأعمدة الفردية في ورقة العمل هذه.

```csharp
public ColumnCollection Columns { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عيّن النمط للعمود 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // عيّن العرض للعمود 5
            cells.Columns[5].Width = 20;

            // عيّن البيانات في العمود 5 لتوضيح النمط
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // احفظ المصنف
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


