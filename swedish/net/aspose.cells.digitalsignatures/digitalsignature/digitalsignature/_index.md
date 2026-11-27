---
title: "DigitalSignature.DigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-konstruktor. Konstruktor för digitalSignature. Använder .Net-implementation"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Konstruktor för digitalSignature. Använder .Net-implementation.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| certifikat | X509Certificate2 | Certifikatobjekt som användes för att signera dokumentet. |
| kommentarer | String | Syftet med signaturen. |
| signTime | DateTime | Den UTC-tiden då dokumentet signerades. |

### Exempel

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
            // Skapa en digital signatursamling
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Läs in certifikat med privat nyckel
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Skapa digital signatur med certifikat, syfte och tidsstämpel
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Skapa en ny arbetsbok och signera den
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Konstruktor för digitalSignature. Använder Bouncy Castle-implementation.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rawData | Byte[] | En byte-array som innehåller data från ett X.509-certifikat. |
| lösenord | String | Lösenordet som krävs för att komma åt X.509-certifikatdata. |
| kommentarer | String | Syftet med signaturen. |
| signTime | DateTime | Den UTC-tiden då dokumentet signerades. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Läs in certifikatfilen som en byte-array (ersätt med den faktiska certifikatvägen)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Skapa parametrar för digital signatur
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Anropa konstruktorn med (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Skapa en DigitalSignatureCollection och lägg till signaturen i den
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Lägg till signaturer i arbetsboken
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


