---
title: "Workbook.AddDigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Fügt einer OOXML-Tabellendatei (Excel2007 und neuer) eine digitale Signatur hinzu"
type: docs
url: /de/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Fügt einer OOXML‑Tabellendatei (Excel2007 und neuer) eine digitale Signatur hinzu.

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Hinweise

Unterstützt nur das Hinzufügen einer Xmldsig-Digital Signatur zu einer OOXML-Tabellendatei

### Beispiele

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einige Beispieldaten hinzu
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Zertifikat laden (ersetzen Sie es durch Ihren eigenen Zertifikatspfad und Ihr Passwort)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Digitale Signatur erstellen
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Digitale Signatursammlung erstellen und Signatur hinzufügen
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Digitale Signatur zum Arbeitsbuch hinzufügen
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Speichere die Arbeitsmappe
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Siehe auch

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


