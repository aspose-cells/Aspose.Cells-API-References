---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsSaveOptions‑egenskap. Anger om ods‑filen ska sparas som ODF‑format version 1.1. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

Anger om ods‑filen ska sparas som ODF‑format version 1.1. Standardvärdet är falskt.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället OdsSaveOptions.OdfStrictVersion‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med februari 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyIsStrictSchema11Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample ODS with strict schema");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.IsStrictSchema11 = true;
            
            workbook.Save("StrictSchema11Example.ods", saveOptions);
        }
    }
}
```

### Se även

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


