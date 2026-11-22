---
title: "Worksheet.TextBoxes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على مجموعة TextBox"
type: docs
url: /ar/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

يحصل على مجموعة [`TextBox`](../../../aspose.cells.drawing/textbox/).

```csharp
public TextBoxCollection TextBoxes { get; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTextBoxesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // عيّن النص وقم بتنسيق أجزائه
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // احفظ المصنف
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


