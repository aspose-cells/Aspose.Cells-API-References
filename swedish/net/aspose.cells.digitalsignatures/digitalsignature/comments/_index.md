---
title: "DigitalSignature.Comments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. Syftet med signaturen"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

Syftet med signaturen.

```csharp
public string Comments { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyCommentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite exempeldata
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Skapa digital signatur med kommentarer
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Lägg till signatur i samlingen
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Signera arbetsboken
            workbook.SetDigitalSignature(dsCollection);

            // Spara den signerade arbetsboken
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Verifiera och visa signaturinformation
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
            }
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


