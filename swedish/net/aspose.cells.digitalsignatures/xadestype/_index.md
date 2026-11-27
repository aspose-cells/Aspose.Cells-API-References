---
title: "Enum XAdESType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DigitalSignatures.XAdESType enum. Typ av XML Advanced Electronic Signature XAdES"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Typ av XML Advanced Electronic Signature (XAdES).

```csharp
public enum XAdESType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | XAdES är av |
| XAdES | `1` | Grundläggande XAdES. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;
    using System.Security.Cryptography.X509Certificates;

    public class XAdESTypeDemo
    {
        public static void XAdESTypeExample()
        {
            // Källkatalog
            string sourceDir = "path_to_source_directory";
            // Utkatalog
            string outputDir = "path_to_output_directory";
            // Läs in arbetsboken
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Definiera lösenordet för PFX-filen
            string password = "pfxPassword";
            // Sökväg till PFX-filen
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Skapa en digital signatur
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Ställ in XAdES-typen
            signature.XAdESType = XAdESType.XAdES;

            // Skapa en samling av digitala signaturer
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Ställ in den digitala signaturen i arbetsboken
            workbook.SetDigitalSignature(dsCollection);

            // Spara arbetsboken med den digitala signaturen
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Verifiera den digitala signaturen
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
    }
}
```

### Se även

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


