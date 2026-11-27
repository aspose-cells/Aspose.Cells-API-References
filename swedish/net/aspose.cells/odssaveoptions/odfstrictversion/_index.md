---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsSaveOptions egenskap. Hämtar och anger ODF-versionen"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Hämtar och anger ODF‑versionen.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // Skapa ODS-sparalternativ
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // Ställ in ODF-versionen till 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Spara med specificerad ODF-version
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Ändra till ODF-version 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Se även

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


