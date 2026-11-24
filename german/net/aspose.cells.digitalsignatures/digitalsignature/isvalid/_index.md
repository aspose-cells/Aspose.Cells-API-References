---
title: "DigitalSignature.IsValid"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature property. Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert true."
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert wahr.

```csharp
public bool IsValid { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System.IO;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIsValidDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Speichern Sie zuerst die Arbeitsmappe.
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Eine digitale Signatursammlung erstellen
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Eine digitale Signatur erstellen (im realen Szenario ein gültiges Zertifikat verwenden)
            // Der erste Parameter sollte ein byte[] mit den Zertifikatsdaten sein
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Signiere die Arbeitsmappe
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Überprüfen Sie die Signatur
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection loadedSignatures = signedWorkbook.GetDigitalSignature();
            
            foreach (DigitalSignature sig in loadedSignatures)
            {
                Console.WriteLine("Signature is valid: " + sig.IsValid);
            }
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


