---
title: "Cells.ApplyColumnStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تطبق تنسيقات على عمود كامل"
type: docs
url: /ar/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

يطبق التنسيقات على عمود كامل.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| النمط | النمط | كائن النمط الذي سيُطبق. |
| علامة | StyleFlag | العلامات التي تشير إلى خصائص التنسيق المطبقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء نمط مع حدود
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // إنشاء علامة نمط لتطبيق الحدود فقط
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // تطبيق النمط على العمود 1 (الفهرس 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // احفظ المصنف
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


