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
// Called: Console.WriteLine($"Sign Time: {ds.SignTime}");
public static void Property_SignTime()
        {
            // Source directory
            string sourceDir = "path_to_source_directory";
            // Output directory
            string outputDir = "path_to_output_directory";
            // Load the workbook
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Define the password for the PFX file
            string password = "pfxPassword";
            // Path to the PFX file
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Create a digital signature
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Set the XAdES type
            signature.XAdESType = XAdESType.XAdES;

            // Create a collection of digital signatures
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Set the digital signature to the workbook
            workbook.SetDigitalSignature(dsCollection);

            // Save the workbook with the digital signature
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Verify the digital signature
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
                Console.WriteLine($"XAdES Type: {ds.XAdESType}");
            }
        }
```

### See Also

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


