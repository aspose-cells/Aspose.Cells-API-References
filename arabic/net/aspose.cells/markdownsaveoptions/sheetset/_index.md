---
title: "MarkdownSaveOptions.SheetSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. تحصل أو تضبط الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف Active"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

تحصل أو تضبط الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### ملاحظات

يتم تجاهل المجموعة عندما تُستخدم في [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // إضافة ورقة عمل ثانية
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // إنشاء خيارات حفظ Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // حفظ جميع الأوراق إلى markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // حفظ الورقة الأولى فقط
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


