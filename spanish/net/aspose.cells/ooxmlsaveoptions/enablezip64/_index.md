---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Utiliza extensiones ZIP64 al escribir archivos zip según sea necesario"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Usar extensiones ZIP64 al escribir archivos zip, según sea necesario.

```csharp
public bool EnableZip64 { get; set; }
```

### Ejemplos

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

### Ver también

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


