---
title: "PdfSecurityOptions.ExtractContentPermissionObsolete"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Permission de copier ou d'extraire du contenu, obsolète selon la référence PDF"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/
---
## PdfSecurityOptions.ExtractContentPermissionObsolete property

Permission de copier ou d'extraire du contenu, obsolète selon la référence PDF.

```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ExtractContentPermission. Cette propriété sera supprimée 12 mois plus tard, depuis septembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionObsoleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.ExtractContentPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("SecurePDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermissionObsolete set to false");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


