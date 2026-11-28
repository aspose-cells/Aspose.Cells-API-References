---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Hücre yazı tipi bununla uyumlu olmadığında yalnızca karakterin yazı tipini değiştirme gerekip gerekmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Hücre yazı tipi uyumlu olmadığında yalnızca karakterin yazı tipini değiştirmeyi gösterir.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Açıklamalar

Varsayılan false'tur. Önce Çalışma Kitabı ve PdfSaveOption/sisteminin varsayılan yazı tipini hücre yazı tipi için deneyeceğiz.

### Örnekler

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

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


