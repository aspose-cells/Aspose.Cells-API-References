---
title: "Classe PdfSecurityOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions class. Opzioni per la crittografia e i permessi di accesso per un documento PDF. PDF/A non consente impostazioni di sicurezza"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Opzioni per la crittografia e i permessi di accesso per un documento PDF. PDF/A non consente impostazioni di sicurezza.

```csharp
public class PdfSecurityOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | Il costruttore di PdfSecurityOptions |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Indica se consentire l'assemblaggio del documento (inserire, ruotare o eliminare pagine e creare segnalibri o immagini in miniatura), anche se [`ModifyDocumentPermission`](./modifydocumentpermission/) è attivo. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Indica se consentire la copia o l'estrazione di testo e grafica dal documento mediante operazioni diverse da quelle controllate da [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsoleto.**) Permesso di copiare o estrarre contenuto Obsoleto secondo il riferimento PDF. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Indica se consentire la compilazione di campi di modulo interattivi esistenti (inclusi i campi firma), anche se [`ModifyDocumentPermission`](./modifydocumentpermission/) è attivo. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Indica se consentire la stampa del documento in una rappresentazione da cui possa essere generata una fedele copia digitale del contenuto PDF. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Indica se consentire la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) e [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Ottiene o imposta la password del proprietario per il documento PDF crittografato. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Indica se consentire la stampa del documento. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Ottiene o imposta la password utente necessaria per aprire il documento PDF crittografato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Crea PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Crea PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Imposta le opzioni di sicurezza
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // Assegna le opzioni di sicurezza a PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Salva la cartella di lavoro come PDF con le opzioni di sicurezza specificate
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


