---
title: "PdfSecurityOptions.UserPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSecurityOptions. Obtient ou définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré"
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Obtient ou définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré.

```csharp
public string UserPassword { get; set; }
```

### Remarques

Le mot de passe propriétaire ou le mot de passe utilisateur sera requis pour ouvrir un document PDF chiffré en vue.

Le mot de passe utilisateur peut être nul ou une chaîne vide ; dans ce cas aucun mot de passe ne sera demandé à l'utilisateur lors de l'ouverture du document PDF.

Ouvrir le document avec le mot de passe propriétaire correct permet un accès complet au document.

Ouvrir le document avec le mot de passe utilisateur correct (ou ouvrir un document qui ne possède pas de mot de passe utilisateur) permet un accès limité selon les autorisations spécifiées.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


