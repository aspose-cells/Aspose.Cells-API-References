---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Используйте расширения ZIP64 при необходимости при записи zip‑архивов"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Использовать расширения ZIP64 при записи zip‑архивов, при необходимости.

```csharp
public bool EnableZip64 { get; set; }
```

### Примеры

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

### См. также

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


