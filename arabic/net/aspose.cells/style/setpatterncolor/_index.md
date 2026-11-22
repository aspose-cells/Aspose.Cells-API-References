---
title: "Style.SetPatternColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تعيين لون الخلفية"
type: docs
url: /ar/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

يضبط لون الخلفية.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نمط | BackgroundType | النمط. |
| color1 | اللون | لون المقدمة. |
| color2 | اللون | لون الخلفية. يعمل فقط عندما لا يكون النمط BackgroundType.None و BackgroundType.Solid. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


