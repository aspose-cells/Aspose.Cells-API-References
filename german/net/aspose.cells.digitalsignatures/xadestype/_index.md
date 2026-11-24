---
title: "Aufzählung XAdESType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DigitalSignatures.XAdESType Enum. Typ der XML Advanced Electronic Signature XAdES"
type: docs
url: /de/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Typ der XML Advanced Electronic Signature (XAdES).

```csharp
public enum XAdESType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | XAdES ist deaktiviert. |
| XAdES | `1` | Basis‑XAdES. |

### Beispiele

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
            // Quellverzeichnis
            string sourceDir = "path_to_source_directory";
            // Ausgabeverzeichnis
            string outputDir = "path_to_output_directory";
            // Laden Sie die Arbeitsmappe
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Definieren Sie das Passwort für die PFX-Datei
            string password = "pfxPassword";
            // Pfad zur PFX-Datei
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Erstellen Sie eine digitale Signatur
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Legen Sie den XAdES-Typ fest
            signature.XAdESType = XAdESType.XAdES;

            // Erstellen Sie eine Sammlung digitaler Signaturen
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Setzen Sie die digitale Signatur in die Arbeitsmappe
            workbook.SetDigitalSignature(dsCollection);

            // Speichern Sie die Arbeitsmappe mit der digitalen Signatur
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Überprüfen Sie die digitale Signatur
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

### Siehe auch

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


