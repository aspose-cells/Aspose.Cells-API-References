---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt an, ob nur die Schriftart eines Zeichens ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Gibt an, ob die Schriftart eines Zeichens nur dann ersetzt werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Hinweise

Standard ist false. Wir versuchen zuerst die Standardschriftart des Arbeitsbuchs und von PdfSaveOption/System für die Zellen-Schriftart.

### Beispiele

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

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


