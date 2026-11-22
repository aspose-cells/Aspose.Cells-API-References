---
title: "Font.IsStrikeout"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. الحصول على أو تعيين قيمة تشير إلى ما إذا كان الخط مشطوبًا مرة واحدة"
type: docs
url: /ar/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط يحتوي على شطب أحادي.

```csharp
public bool IsStrikeout { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الطريقة 1: تعيين التشطيب عبر النمط مباشرة
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // الطريقة 2: تعيين التشطيب عبر HTML
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // تحقق من خاصية التشطيب
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // حفظ للتحقق
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


