---
title: "Style.ForegroundArgbColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Style property. يحصل على ويضبط لون المقدمة باستخدام قيمة ARGB 32 بت"
type: docs
url: /ar/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

يحصل على اللون الأمامي ويضبطه باستخدام قيمة ARGB 32 بت.

```csharp
public int ForegroundArgbColor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط بلون مقدمة محدد
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // احصل على وعرض قيمة لون ARGB للمقدمة
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // احفظ المصنف
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


