---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. استخدم امتدادات ZIP64 عند كتابة أرشيفات zip حسب الضرورة"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

استخدم امتدادات ZIP64 عند كتابة أرشيفات zip، حسب الضرورة.

```csharp
public bool EnableZip64 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEnableZip64Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Sample data for Zip64 demonstration");
            
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EnableZip64 = true;
            
            workbook.Save("output_with_zip64.xlsx", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


