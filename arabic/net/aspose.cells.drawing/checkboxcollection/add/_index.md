---
title: "CheckBoxCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CheckBoxCollection. يضيف checkBox إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

يضيف checkBox إلى المجموعة.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع checkBox، بوحدة البكسل. |
| العرض | Int32 | عرض checkBox، بوحدة البكسل. |

### قيمة الإرجاع

[`CheckBox`](../../checkbox/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف checkBox باستخدام معاملات Int32 (upperLeftRow، upperLeftColumn، الارتفاع، العرض)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


