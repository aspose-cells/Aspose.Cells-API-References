---
title: "DigitalSignature.DigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DigitalSignature. Costruttore di digitalSignature. Utilizza l'implementazione .Net"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Costruttore di digitalSignature. Utilizza l'implementazione .Net.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| certificato | X509Certificate2 | Oggetto certificato utilizzato per firmare il documento. |
| commenti | String | Lo scopo della firma. |
| signTime | DateTime | L'ora UTC in cui il documento è stato firmato. |

### Esempi

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
            // Crea una collezione di firme digitali
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Carica il certificato con chiave privata
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Crea una firma digitale con certificato, scopo e timestamp
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Crea una nuova cartella di lavoro e firmala
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Costruttore di digitalSignature. Utilizza l'implementazione Bouncy Castle.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rawData | Byte[] | Un array di byte contenente dati da un certificato X.509. |
| password | String | La password necessaria per accedere ai dati del certificato X.509. |
| commenti | String | Lo scopo della firma. |
| signTime | DateTime | L'ora UTC in cui il documento è stato firmato. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi del contenuto di esempio
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Carica il file del certificato come array di byte (sostituisci con il percorso reale del certificato)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Crea i parametri della firma digitale
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Chiama il costruttore con (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Crea una DigitalSignatureCollection e aggiungi la firma ad essa
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Aggiungi firme alla cartella di lavoro
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


