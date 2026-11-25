---
title: "DigitalSignature.IsValid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà true.

```csharp
public bool IsValid { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati al worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Salva prima la cartella di lavoro
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Crea una collezione di firme digitali
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Crea una firma digitale (in uno scenario reale, usa un certificato appropriato)
            // Il primo parametro dovrebbe essere byte[] dei dati del certificato
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Firma la cartella di lavoro
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Verifica la firma
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

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


