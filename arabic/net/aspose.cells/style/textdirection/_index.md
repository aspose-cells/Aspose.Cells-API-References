---
title: "Style.TextDirection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Style property. يمثل ترتيب قراءة النص"
type: docs
url: /ar/net/aspose.cells/style/textdirection/
---
## Style.TextDirection property

يمثل ترتيب قراءة النص.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyTextDirectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين اتجاهات نصية مختلفة
            Style style1 = cells["A1"].GetStyle();
            style1.TextDirection = TextDirectionType.Context;
            cells["A1"].SetStyle(style1);
            cells["A1"].PutValue("Context Direction");

            Style style2 = cells["A2"].GetStyle();
            style2.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style2);
            cells["A2"].PutValue("LeftToRight Direction");

            Style style3 = cells["A3"].GetStyle();
            style3.TextDirection = TextDirectionType.RightToLeft;
            cells["A3"].SetStyle(style3);
            cells["A3"].PutValue("RightToLeft Direction");

            // احفظ المصنف
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextDirectionType](../../textdirectiontype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


