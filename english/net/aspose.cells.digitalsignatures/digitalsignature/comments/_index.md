---
title: DigitalSignature.Comments
second_title: Aspose.Cells for .NET API Reference
description: DigitalSignature property. The purpose to signature
type: docs
url: /net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

The purpose to signature.

```csharp
public string Comments { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Comments: &amp;quot; + existingDs.Comments);
public static void Property_Comments()
        {
            // Load a workbook from a signed source file
            Workbook signedWorkbook = new Workbook(@&quot;DigitalSignatureCollection_original.xlsx&quot;);

            // Check if the workbook is digitally signed
            Console.WriteLine(&quot;Is the workbook digitally signed? &quot; + signedWorkbook.IsDigitallySigned);

            // Get the digital signature collection from the workbook
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Iterate over the digital signatures in the collection
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine(&quot;Comments: &quot; + existingDs.Comments);
                    Console.WriteLine(&quot;Sign Time: &quot; + existingDs.SignTime);
                    Console.WriteLine(&quot;Is Valid: &quot; + existingDs.IsValid);
                }

                // Create a new digital signature
                X509Certificate2 certificate = new X509Certificate2(&quot;path_to_certificate.pfx&quot;, &quot;password&quot;);
                DigitalSignature newSignature = new DigitalSignature(certificate, &quot;New signature comment&quot;, DateTime.Now);

                // Add the new digital signature to the collection
                existingDsc.Add(newSignature);
            }     
            

            // Save the workbook with the new digital signature
            signedWorkbook.Save(&quot;DigitalSignatureCollectionExample.xlsx&quot;);
            signedWorkbook.Save(&quot;DigitalSignatureCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


