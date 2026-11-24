---
title: "DigitalSignature.DigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature-Konstruktor. Konstruktor von digitalSignature. Verwendet .Net-Implementierung"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Konstruktor von digitalSignature. Verwendet .Net-Implementierung.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zertifikat | X509Certificate2 | Zertifikatsobjekt, das zum Signieren des Dokuments verwendet wurde. |
| Kommentare | String | Der Zweck der Signatur. |
| signTime | DateTime | Die UTC-Zeit, zu der das Dokument signiert wurde. |

### Beispiele

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // Eine digitale Signatursammlung erstellen
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Lade Zertifikat mit privatem Schlüssel
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Erstelle digitale Signatur mit Zertifikat, Zweck und Zeitstempel
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Erstelle eine neue Arbeitsmappe und signiere sie
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Konstruktor von digitalSignature. Verwendet Bouncy‑Castle-Implementierung.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rawData | Byte[] | Ein Byte-Array, das Daten aus einem X.509-Zertifikat enthält. |
| Passwort | String | Das Passwort, das zum Zugriff auf die X.509-Zertifikatsdaten erforderlich ist. |
| Kommentare | String | Der Zweck der Signatur. |
| signTime | DateTime | Die UTC-Zeit, zu der das Dokument signiert wurde. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge etwas Beispielinhalt hinzu
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Lade Zertifikatsdatei als Byte-Array (ersetze durch tatsächlichen Zertifikatspfad)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Erstelle Parameter für digitale Signatur
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Rufe den Konstruktor mit (Byte[], String, String, DateTime) auf
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Erstelle eine DigitalSignatureCollection und füge die Signatur hinzu
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Füge Signaturen zum Arbeitsbuch hinzu
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


