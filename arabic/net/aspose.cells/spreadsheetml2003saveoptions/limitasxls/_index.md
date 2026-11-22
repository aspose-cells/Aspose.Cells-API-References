---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SpreadsheetML2003SaveOptions. الحد كملف xls حيث الحد الأقصى لفهرس الصف هو 65535 والحد الأقصى لفهرس العمود هو 255"
type: docs
url: /ar/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

الحد كملف xls، الحد الأقصى لفهرس الصف هو 65535 والحد الأقصى لفهرس العمود هو 255.

```csharp
public bool LimitAsXls { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // الوصول إلى الخلايا وإنشاء نطاق
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // حفظ مع LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // حفظ كـ SpreadsheetML مع حدود XLS
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### انظر أيضًا

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


