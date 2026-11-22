---
title: "Workbook.CreateBuiltinStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تنشئ نمطًا مدمجًا بالنوع المحدد"
type: docs
url: /ar/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

ينشئ نمطًا مدمجًا حسب النوع المحدد.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | BuiltinStyleType | النمط المدمج. |

### قيمة الإرجاع

[`Style`](../../style/) object

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateBuiltinStyleWithBuiltinStyleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // تطبيق النمط المدمج الجيد
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // تطبيق النمط المدمج المحايد
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // احفظ المصنف
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


