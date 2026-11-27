---
title: "VbaProject.CertRawData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject-egenskap. Hämtar certifikatets rådata om detta VBA-projekt är signerat"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Hämtar certifikatets rådata om detta VBA-projekt är signerat.

```csharp
public byte[] CertRawData { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok med VBA-projekt
            Workbook workbook = new Workbook();
            // Ingen anledning att skapa ett nytt VbaProject eftersom Workbook redan har ett

            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;

            // Kontrollera om VBA-projektet är signerat
            if (vbaProject.IsSigned)
            {
                // Visa certifikatets rådata om signerat
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Exempel: Spara certifikatsdata till fil om den finns
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

            // Exempelscenario: Läs in en arbetsbok med signerat VBA-projekt
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

            // Spara arbetsboken
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


