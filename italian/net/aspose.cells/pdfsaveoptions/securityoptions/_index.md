---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions proprietà. Imposta queste opzioni quando è necessaria la sicurezza nel risultato xls2pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Configura le opzioni di sicurezza
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Assegna le opzioni di sicurezza alle opzioni di salvataggio
            saveOptions.SecurityOptions = securityOptions;
            
            // Salva il PDF con le impostazioni di sicurezza
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Vedi anche

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


