---
title: "Cells.ApplyRowStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تطبق تنسيقات لصف كامل"
type: docs
url: /ar/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

يطبق التنسيقات على الصف بأكمله.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| النمط | النمط | كائن النمط الذي سيُطبق. |
| علامة | StyleFlag | العلامات التي تشير إلى خصائص التنسيق المطبقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نمط مع حدود
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // إنشاء علم نمط للحدود
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // تطبيق النمط على الصف الأول
            cells.ApplyRowStyle(0, style, styleFlag);

            // احفظ المصنف
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


