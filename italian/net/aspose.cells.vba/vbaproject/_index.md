---
title: "Classe VbaProject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Vba.VbaProject. Rappresenta il progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Rappresenta il progetto VBA.

```csharp
public class VbaProject
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Ottiene i dati grezzi del certificato se questo progetto VBA è firmato. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Ottiene e imposta la codifica del progetto VBA. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Indica se questo progetto VBA è bloccato per la visualizzazione. Se vero, i codici non possono essere visibili. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Indica se questo progetto VBA è bloccato per la visualizzazione. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Indica se questo progetto VBA è protetto. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Indica se il codice VBA è firmato o meno. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Indica se la firma del progetto VBA è valida o meno. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Ottiene tutti gli oggetti [`VbaModule`](../vbamodule/). |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Ottiene e imposta il nome del progetto VBA. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Ottiene tutti i riferimenti del progetto VBA. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Copia il progetto VBA da un altro file. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Protegge o rimuove la protezione di questo progetto VBA. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Firma questo progetto VBA con una DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Convalida la password di protezione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Text;
    using System.Security.Cryptography.X509Certificates;

    public class VbaProjectDemo
    {
        public static void VbaProjectExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Inizializza progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Impostazione delle proprietà
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Verifica le proprietà di sola lettura.
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Aggiunta di un modulo VBA
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Aggiunta di un riferimento al progetto VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Protezione del progetto VBA
            vbaProject.Protect(true, "password");

            // Firma del progetto VBA
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Salvataggio del file Excel
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


