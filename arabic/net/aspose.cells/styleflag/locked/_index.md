---
title: "StyleFlag.Locked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد القفل"
type: docs
url: /ar/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

سيتم تطبيق إعداد القفل.

```csharp
public bool Locked { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نمط وتعيين خاصية القفل الخاصة به
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // إنشاء علامة نمط وتمكين علامة القفل
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // تطبيق النمط على الخلية A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // تحقق من حالة القفل
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // حماية ورقة العمل لرؤية تأثير القفل
            worksheet.Protect(ProtectionType.All);

            // حاول تعديل الخلية المقفلة (سيتم إلقاء استثناء عندما تكون ورقة العمل محمية)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


