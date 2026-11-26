---
title: "DigitalSignature.Comments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. El propósito de la firma"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

El propósito de la firma.

```csharp
public string Comments { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos de ejemplo
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Crear firma digital con comentarios
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Agregar firma a la colección
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Firmar el libro de trabajo
            workbook.SetDigitalSignature(dsCollection);

            // Guardar el libro de trabajo firmado
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Verificar y mostrar información de la firma
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

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


