---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PptxSaveOptions property. Inidicates whether ignoring hidden rows when converting Excel to PowerPoint"
type: docs
url: /ar/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

يشير إلى ما إذا كان سيتم تجاهل الصفوف المخفية عند تحويل Excel إلى PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data and hide some rows
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Hide row 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Set PPTX save options with IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // حفظ كـ PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### انظر أيضًا

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


