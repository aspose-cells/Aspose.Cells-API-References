---
title: "Workbook.SetDigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Setzt eine digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer)"
type: docs
url: /de/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Setzt eine digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Hinweise

Unterstützt nur das Hinzufügen von Xmldsig-Digital Signaturen

### Beispiele

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
            // Quellverzeichnis-Pfad
            string sourceDir = "SourceDirectory/";
            
            // Pfad des Ausgabeverzeichnisses
            string outputDir = "OutputDirectory/";

            // Laden Sie die Arbeitsmappe
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Digitale Signatursammlung erstellen
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Zertifikatsdatei laden
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Digitale Signatur erstellen
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Signatur zur Sammlung hinzufügen
            digitalSignatures.Add(signature);

            // Digitale Signatur dem Workbook zuweisen
            workbook.SetDigitalSignature(digitalSignatures);

            // Speichere die Arbeitsmappe
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Siehe auch

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


