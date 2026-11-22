---
title: "SheetSet.All"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetSet. تُرجع مجموعة تحتوي على جميع أوراق دفتر العمل بترتيبها الأصلي"
type: docs
url: /ar/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

يحصل على مجموعة تحتوي على جميع أوراق المصنف بترتيبها الأصلي.

```csharp
public static SheetSet All { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // إنشاء مصنف يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // اضبط بعض البيانات النموذجية في كلا الورقتين
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // حفظ جميع الأوراق إلى markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


