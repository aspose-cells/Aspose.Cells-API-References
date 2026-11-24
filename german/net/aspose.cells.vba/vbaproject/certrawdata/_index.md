---
title: "VbaProject.CertRawData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt die rohen Zertifikatsdaten zurück, wenn dieses VBA-Projekt signiert ist"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Liest die rohen Zertifikatsdaten, wenn dieses VBA-Projekt signiert ist.

```csharp
public byte[] CertRawData { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook();
            // Kein Bedarf, ein neues VbaProject zu erstellen, da das Workbook bereits eines hat

            // Zugriff auf das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;

            // Überprüfen Sie, ob das VBA-Projekt signiert ist.
            if (vbaProject.IsSigned)
            {
                // Zertifikatsrohdaten anzeigen, wenn signiert
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Beispiel: Zertifikatsdaten in Datei speichern, falls vorhanden
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // Beispielszenario: Laden Sie ein Workbook mit signiertem VBA-Projekt
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


