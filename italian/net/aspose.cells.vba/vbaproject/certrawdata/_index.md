---
title: "VbaProject.CertRawData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Ottiene i dati grezzi del certificato se questo progetto VBA è firmato"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Ottiene i dati grezzi del certificato se questo progetto VBA è firmato.

```csharp
public byte[] CertRawData { get; }
```

### Esempi

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
            // Crea una nuova cartella di lavoro con progetto VBA
            Workbook workbook = new Workbook();
            // Non è necessario creare un nuovo VbaProject poiché Workbook ne ha già uno

            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Verifica se il progetto VBA è firmato
            if (vbaProject.IsSigned)
            {
                // Visualizza i dati grezzi del certificato se firmato
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Esempio: salva i dati del certificato su file se esiste
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

            // Scenario di esempio: carica un workbook con progetto VBA firmato
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

            // Salva la cartella di lavoro
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


