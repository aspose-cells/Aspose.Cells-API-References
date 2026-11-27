---
title: "DigitalSignature.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature property. Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Tomt"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Empty.

```csharp
public string Text { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett testcertifikat (i verkligt scenario, använd ett giltigt certifikat)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Skapa en digital signaturinstans
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Visa det aktuella Text-värdet (standard är tomt)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Ställ in ett nytt värde för Text-egenskapen
            signature.Text = "Approved by John Doe";

            // Skapa en digital signatursamling och lägg till signaturen i den
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Lägg till de digitala signaturerna i arbetsboken
            workbook.AddDigitalSignature(signatures);

            // Spara arbetsboken med digital signatur
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

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


