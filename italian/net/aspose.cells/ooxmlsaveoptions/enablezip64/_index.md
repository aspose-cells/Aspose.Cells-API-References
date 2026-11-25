---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Usa le estensioni ZIP64 quando si scrivono archivi zip, se necessario"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Usa le estensioni ZIP64 quando scrivi archivi zip, se necessario.

```csharp
public bool EnableZip64 { get; set; }
```

### Esempi

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

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


