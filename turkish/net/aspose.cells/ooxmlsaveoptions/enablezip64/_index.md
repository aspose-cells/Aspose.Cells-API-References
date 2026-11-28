---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions özelliği. Zip arşivleri yazılırken gerektiğinde ZIP64 uzantılarını kullan"
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Gerekli olduğunda zip arşivleri yazarken ZIP64 uzantılarını kullan.

```csharp
public bool EnableZip64 { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


