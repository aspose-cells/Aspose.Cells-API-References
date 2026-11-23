---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte ainsi que le remplissage de champs de formulaire interactifs"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Remarques

si [`ModifyDocumentPermission`](../modifydocumentpermission/) est également définie, créer ou modifier des champs de formulaire interactifs (y compris les champs de signature).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.AnnotationsPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with annotations permission enabled.");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


