---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser l'assemblage du document, l'insertion, la rotation ou la suppression de pages, ainsi que la création de signets ou d'images miniatures, même si ModifyDocumentPermission est autorisée"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [`ModifyDocumentPermission`](../modifydocumentpermission/) est autorisée.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


