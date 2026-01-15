---
title: Class DigitalSignature
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.DigitalSignatures.DigitalSignature class. Signature in file
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Signature in file.

```csharp
public class DigitalSignature
```

## Constructors

| Name | Description |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Constructor of digitalSignature. Uses .Net implementation. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Constructor of digitalSignature. Uses Bouncy Castle implementation. |

## Properties

| Name | Description |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Certificate object that was used to sign the document. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | The purpose to signature. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Specifies an image for the digital signature. Default value is null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | The time when the document was signed. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | XAdES type. Default value is None(XAdES is off). |

### Examples

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
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Create a digital signature using certificate constructor
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Set additional properties
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Add signature to workbook
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Display signature information
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Save the signed workbook
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

### See Also

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


