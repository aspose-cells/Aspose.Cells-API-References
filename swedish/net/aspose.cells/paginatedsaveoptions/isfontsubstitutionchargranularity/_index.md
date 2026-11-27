---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions‑egenskap. Anger om endast tecknets teckensnitt ska ersättas när cellens teckensnitt inte är kompatibelt."
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Anmärkningar

Standard är false. Vi kommer först att prova standardteckensnittet för Workbook och PdfSaveOption/system för cellens teckensnitt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Sample Text with Font Substitution");

            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                IsFontSubstitutionCharGranularity = true,
                DefaultFont = "Arial"
            };

            workbook.Save("FontSubstitutionDemo.xps", saveOptions);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


