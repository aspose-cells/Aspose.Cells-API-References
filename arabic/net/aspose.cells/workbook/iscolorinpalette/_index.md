---
title: "Workbook.IsColorInPalette"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تتحقق مما إذا كان اللون موجودًا في لوحة الألوان للجدول"
type: docs
url: /ar/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

يتحقق مما إذا كان اللون موجودًا في لوحة ألوان جدول البيانات.

```csharp
public bool IsColorInPalette(Color color)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | بنية اللون. |

### قيمة الإرجاع

يرجع true إذا كان هذا اللون موجودًا في لوحة الألوان. وإلا، يرجع false

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // تحقق مما إذا كان اللون القياسي موجودًا في لوحة الألوان
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // تحقق مما إذا كان اللون المخصص موجودًا في لوحة الألوان
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // احصل على اللون المطابق من لوحة الألوان
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


