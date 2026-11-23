---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par AnnotationsPermission, FillFormsPermission et AssembleDocumentPermission"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) et [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // Configurez les options d'enregistrement PDF avec les paramètres de sécurité
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Définissez les mots de passe et les autorisations
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Appliquez les options de sécurité et enregistrez
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


