---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor DifSaveOptions. Crea las opciones para guardar un archivo DIF"
type: docs
url: /es/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Crea las opciones para guardar un archivo DIF.

```csharp
public DifSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DifSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            DifSaveOptions saveOptions = new DifSaveOptions()
            {
                ClearData = true,
                CreateDirectory = true,
                RefreshChartCache = true
            };

            workbook.Save("DifSaveOptionsOutput.dif", saveOptions);
        }
    }
}
```

### Ver también

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


