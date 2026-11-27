---
title: "Klass VbaProject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Vba.VbaProject-klass. Representerar VBA-projektet"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Representerar VBA‑projektet.

```csharp
public class VbaProject
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Hämtar certifikatets rådata om detta VBA-projekt är signerat. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Hämtar och anger kodningen för VBA-projektet. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Anger om detta VBA-projekt är låst för visning. Om true, kan koden inte vara synlig. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Anger om detta VBA-projekt är låst för visning. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Anger om detta VBA-projekt är skyddat. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Anger om VBA-kod är signerat eller inte. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Anger om signaturen för VBA-projektet är giltig eller inte. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Hämtar alla [`VbaModule`](../vbamodule/) objekt. |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Hämtar och anger namnet på VBA-projektet. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Hämtar alla referenser för VBA-projektet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Kopiera VBA-projekt från en annan fil. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Skyddar eller avskyddar detta VBA-projekt. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Signera detta VBA-projekt med en DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Validerar skyddslösenordet. |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Initiera VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Ställa in egenskaper
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Kontrollerar skrivskyddade egenskaper
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Lägger till en VBA-modul
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Lägger till en VBA-projektreferens
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Skyddar VBA-projektet
            vbaProject.Protect(true, "password");

            // Signerar VBA-projektet
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Sparar Excel-filen
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


