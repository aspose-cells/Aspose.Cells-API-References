---
title: "DigitalSignature.IsValid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature property. Om denna digitala signatur är giltig och dokumentet inte har manipulerats kommer detta värde att vara sant"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Om denna digitala signatur är giltig och dokumentet inte har manipulerats, kommer detta värde att vara true.

```csharp
public bool IsValid { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Spara arbetsboken först
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Skapa en digital signatursamling
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Skapa en digital signatur (i verkligt scenario, använd korrekt certifikat)
            // Första parametern bör vara byte[] med certifikatdata
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Signera arbetsboken
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Verifiera signaturen
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

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


