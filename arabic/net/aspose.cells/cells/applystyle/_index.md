---
title: "Cells.ApplyStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تطبيق تنسيقات على ورقة عمل كاملة"
type: docs
url: /ar/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

يطبق التنسيقات على ورقة عمل كاملة.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | كائن النمط الذي سيُطبق. |
| علامة | StyleFlag | العلامات التي تشير إلى خصائص التنسيق المطبقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء نمط وتعيين التفاف النص
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // إنشاء علم النمط وتمكين علم التفاف النص
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // تطبيق النمط على جميع الخلايا في ورقة العمل
            sheet.Cells.ApplyStyle(style, flag);
            
            // احفظ المصنف
            wb.Save("output.xlsx", SaveFormat.Xlsx);
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


