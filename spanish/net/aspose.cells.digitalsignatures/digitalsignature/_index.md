---
title: "Clase DigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DigitalSignatures.DigitalSignature. Firma en el archivo"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Firma en el archivo.

```csharp
public class DigitalSignature
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Constructor de digitalSignature. Utiliza la implementación de .Net. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Constructor de digitalSignature. Utiliza la implementación de Bouncy Castle. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Objeto de certificado que se utilizó para firmar el documento. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | El propósito de la firma. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Especifica un GUID que puede ser referenciado cruzadamente con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Especifica una imagen para la firma digital. El valor predeterminado es null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Si esta firma digital es válida y el documento no ha sido manipulado, este valor será true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | La hora en que se firmó el documento. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | Tipo XAdES. El valor predeterminado es None (XAdES está desactivado). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Crear una firma digital usando el constructor de certificado
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Establecer propiedades adicionales
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Agregar firma al libro de trabajo
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Mostrar información de la firma
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Guardar el libro de trabajo firmado
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


