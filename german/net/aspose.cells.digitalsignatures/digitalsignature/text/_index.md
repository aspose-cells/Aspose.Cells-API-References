---
title: "DigitalSignature.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature property. Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist leer."
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist Empty.

```csharp
public string Text { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein Testzertifikat erstellen (im realen Szenario ein gültiges Zertifikat verwenden)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Eine Instanz einer digitalen Signatur erstellen
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Den aktuellen Textwert anzeigen (Standard ist leer)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Einen neuen Wert für die Text‑Eigenschaft festlegen
            signature.Text = "Approved by John Doe";

            // Eine digitale Signatursammlung erstellen und die Signatur hinzufügen
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Die digitalen Signaturen zur Arbeitsmappe hinzufügen
            workbook.AddDigitalSignature(signatures);

            // Die Arbeitsmappe mit digitaler Signatur speichern
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

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


