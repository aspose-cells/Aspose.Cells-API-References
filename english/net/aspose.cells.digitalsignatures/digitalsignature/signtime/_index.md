---
title: DigitalSignature.SignTime
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. The time when the document was signed
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

The time when the document was signed.

```csharp
public DateTime SignTime { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Sign Time: " + existingDs.SignTime);
public static void DigitalSignature_Property_SignTime()
        {
            // Load a workbook from a signed source file
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Check if the workbook is digitally signed
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Get the digital signature collection from the workbook
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Iterate over the digital signatures in the collection
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Create a new digital signature
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Add the new digital signature to the collection
                existingDsc.Add(newSignature);
            }     
            

            // Save the workbook with the new digital signature
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


