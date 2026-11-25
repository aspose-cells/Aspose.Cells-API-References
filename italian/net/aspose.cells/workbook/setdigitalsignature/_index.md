---
title: "Workbook.SetDigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo del workbook. Imposta la firma digitale su un file di foglio di calcolo Excel2007 e versioni successive"
type: docs
url: /it/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Osservazioni

Supporta solo l'aggiunta di firme digitali Xmldsig

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Percorso della directory di origine
            string sourceDir = "SourceDirectory/";
            
            // Percorso della directory di destinazione
            string outputDir = "OutputDirectory/";

            // Carica la cartella di lavoro
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Crea una raccolta di firme digitali
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Carica il file di certificato
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Crea firma digitale
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Aggiungi la firma alla raccolta
            digitalSignatures.Add(signature);

            // Imposta la firma digitale sul workbook
            workbook.SetDigitalSignature(digitalSignatures);

            // Salva la cartella di lavoro
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Vedi anche

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


