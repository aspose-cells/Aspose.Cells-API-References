---
title: "DigitalSignature.Comments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Lo scopo della firma"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

Lo scopo della firma.

```csharp
public string Comments { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati di esempio
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Crea una firma digitale con commenti
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Aggiungi la firma alla raccolta
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Firma la cartella di lavoro
            workbook.SetDigitalSignature(dsCollection);

            // Salva la cartella di lavoro firmata
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Verifica e visualizza le informazioni della firma
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

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


