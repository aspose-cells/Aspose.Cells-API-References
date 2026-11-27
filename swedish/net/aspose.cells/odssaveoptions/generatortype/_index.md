---
title: "OdsSaveOptions.GeneratorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsSaveOptions‑egenskap. Hämtar och anger generatorn för ods‑filen"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Hämtar och anger generatorn för ods‑filen.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyGeneratorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa och konfigurera ODS‑sparalternativ
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Spara arbetsboken med angivna alternativ
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Se även

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


