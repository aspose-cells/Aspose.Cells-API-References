---
title: "Klasse VbaProject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaProject Klasse. Stellt das VBA-Projekt dar"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Stellt das VBA‑Projekt dar.

```csharp
public class VbaProject
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Liest die rohen Zertifikatsdaten, wenn dieses VBA-Projekt signiert ist. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Liest und setzt die Kodierung des VBA-Projekts. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. Wenn true, sind die Codes nicht sichtbar. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Gibt an, ob dieses VBA-Projekt geschützt ist. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Gibt an, ob VBAcode signiert ist oder nicht. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Liest alle [`VbaModule`](../vbamodule/) Objekte. |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Liest und setzt den Namen des VBA-Projekts. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Liest alle Verweise des VBA-Projekts. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Kopiere VBA-Projekt aus einer anderen Datei. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Schützt oder hebt den Schutz dieses VBA-Projekts auf. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Signiere dieses VBA-Projekt mit einer DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Validiert das Schutzkennwort. |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;

            // Eigenschaften festlegen
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Überprüfen von schreibgeschützten Eigenschaften
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Hinzufügen eines VBA-Moduls
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Hinzufügen einer VBA-Projektreferenz
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Schützen des VBA-Projekts
            vbaProject.Protect(true, "password");

            // Signieren des VBA-Projekts
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Die Excel-Datei speichern
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


