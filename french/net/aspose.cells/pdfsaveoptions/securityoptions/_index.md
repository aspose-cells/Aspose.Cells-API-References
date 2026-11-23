---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Définissez ces options lorsque la sécurité est requise dans le résultat xls2pdf"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Définissez ces options, lorsque la sécurité est requise dans le résultat xls2pdf.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // Créez les options d'enregistrement PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Configurez les options de sécurité
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Attribuez les options de sécurité aux options d'enregistrement
            saveOptions.SecurityOptions = securityOptions;
            
            // Enregistrez le PDF avec les paramètres de sécurité
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Voir aussi

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


