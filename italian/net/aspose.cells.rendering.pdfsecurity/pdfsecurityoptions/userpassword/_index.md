---
title: "PdfSecurityOptions.UserPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSecurityOptions. Ottiene o imposta la password utente necessaria per aprire il documento PDF crittografato"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Ottiene o imposta la password utente necessaria per aprire il documento PDF crittografato.

```csharp
public string UserPassword { get; set; }
```

### Osservazioni

La password del proprietario o la password utente saranno necessarie per aprire un documento PDF crittografato per la visualizzazione.

La password utente può essere null o una stringa vuota; in questo caso non sarà richiesta alcuna password all'utente durante l'apertura del documento PDF.

Aprire il documento con la password del proprietario corretta consente l'accesso completo al documento.

Aprire il documento con la password utente corretta (o aprire un documento che non ha una password utente) consente un accesso limitato secondo le autorizzazioni specificate.

### Esempi

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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


