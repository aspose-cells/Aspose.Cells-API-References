---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF pourrait être générée"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF pourrait être générée.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Remarques

Lorsque elle est autorisée (et que [`PrintPermission`](../printpermission/) est définie), l'impression est limitée à une représentation de bas niveau de l'apparence, éventuellement de qualité dégradée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFullQualityPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Full Quality Print Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FullQualityPrintPermission = true;
            securityOptions.PrintPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("FullQualityPrintDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with FullQualityPrintPermission enabled.");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


