---
title: "DigitalSignature.IsValid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Si esta firma digital es válida y el documento no ha sido manipulado, este valor será verdadero"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Si esta firma digital es válida y el documento no ha sido manipulado, este valor será true.

```csharp
public bool IsValid { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Guarda el libro de trabajo primero
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Crear una colección de firmas digitales
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Crear una firma digital (en un escenario real, use un certificado adecuado)
            // El primer parámetro debe ser byte[] de los datos del certificado
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Firmar el libro de trabajo
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Verificar la firma
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

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


