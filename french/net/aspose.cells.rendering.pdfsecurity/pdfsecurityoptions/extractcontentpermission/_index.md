---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par AccessibilityExtractContent"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [`AccessibilityExtractContent`](../accessibilityextractcontent/).

```csharp
public bool ExtractContentPermission { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // Configurez les options d'enregistrement PDF avec les paramètres de sécurité
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Définissez les mots de passe et les autorisations
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // Démontrez l'utilisation de ExtractContentPermission
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Appliquez les options de sécurité et enregistrez
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


