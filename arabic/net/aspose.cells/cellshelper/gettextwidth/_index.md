---
title: "CellsHelper.GetTextWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. احصل على عرض النص بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

احصل على عرض النص بوحدة النقاط.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | النص. |
| خط | خط | خط النص. |
| تحجيم | Double | تحجيم النص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### انظر أيضًا

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


