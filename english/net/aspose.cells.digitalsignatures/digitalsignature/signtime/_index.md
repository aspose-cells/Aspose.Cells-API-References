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
// Called: Console.WriteLine($&amp;quot;Sign Time: {ds.SignTime}&amp;quot;);
public static void Property_SignTime()
        {
            // Source directory
            string sourceDir = &quot;path_to_source_directory&quot;;
            // Output directory
            string outputDir = &quot;path_to_output_directory&quot;;
            // Load the workbook
            Workbook workbook = new Workbook(Path.Combine(sourceDir, &quot;XAdESTypeExample_original.xlsx&quot;));

            // Define the password for the PFX file
            string password = &quot;pfxPassword&quot;;
            // Path to the PFX file
            string pfxPath = Path.Combine(sourceDir, &quot;pfxFile.pfx&quot;);

            // Create a digital signature
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, &quot;testXAdES&quot;, DateTime.Now);
            // Set the XAdES type
            signature.XAdESType = XAdESType.XAdES;

            // Create a collection of digital signatures
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Set the digital signature to the workbook
            workbook.SetDigitalSignature(dsCollection);

            // Save the workbook with the digital signature
            workbook.Save(Path.Combine(outputDir, &quot;XAdESSignatureSupport_out.xlsx&quot;));

            // Verify the digital signature
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, &quot;XAdESSignatureSupport_out.xlsx&quot;));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($&quot;Comments: {ds.Comments}&quot;);
                Console.WriteLine($&quot;Sign Time: {ds.SignTime}&quot;);
                Console.WriteLine($&quot;Is Valid: {ds.IsValid}&quot;);
                Console.WriteLine($&quot;XAdES Type: {ds.XAdESType}&quot;);
            }
        }
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


