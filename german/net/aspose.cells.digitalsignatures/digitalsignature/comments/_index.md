---
title: "DigitalSignature.Comments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature-Eigenschaft. Der Zweck der Signatur"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

Der Zweck der Signatur.

```csharp
public string Comments { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einige Beispieldaten hinzu
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Erstelle eine digitale Signatur mit Kommentaren
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Signatur zur Sammlung hinzufügen
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Signiere die Arbeitsmappe
            workbook.SetDigitalSignature(dsCollection);

            // Das signierte Arbeitsbuch speichern
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Überprüfe und zeige Signaturinformationen an
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

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


