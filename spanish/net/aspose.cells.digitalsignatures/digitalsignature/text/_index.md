---
title: "DigitalSignature.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Especifica el texto de la firma real en la firma digital. El valor predeterminado es Vacío"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty.

```csharp
public string Text { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un certificado de prueba (en un escenario real, use un certificado válido)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Crear una instancia de firma digital
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Mostrar el valor actual de Text (el predeterminado es vacío)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Establecer un nuevo valor para la propiedad Text
            signature.Text = "Approved by John Doe";

            // Crear una colección de firmas digitales y agregar la firma a ella
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Agregar las firmas digitales al libro de trabajo
            workbook.AddDigitalSignature(signatures);

            // Guardar el libro de trabajo con firma digital
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

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


