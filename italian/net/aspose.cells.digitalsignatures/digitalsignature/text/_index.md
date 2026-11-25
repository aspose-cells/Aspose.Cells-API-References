---
title: "DigitalSignature.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty.

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un certificato di test (in uno scenario reale, usa un certificato valido)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Crea un'istanza di firma digitale
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Visualizza il valore corrente di Text (il valore predefinito è vuoto)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Imposta un nuovo valore per la proprietà Text
            signature.Text = "Approved by John Doe";

            // Crea una raccolta di firme digitali e aggiungi la firma ad essa
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Aggiungi le firme digitali alla cartella di lavoro
            workbook.AddDigitalSignature(signatures);

            // Salva la cartella di lavoro con firma digitale
            try
            {
                workbook.Save("DigitalSignatureWithText.xlsx");
                Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error saving workbook: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


