---
title: "Enum XAdESType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.DigitalSignatures.XAdESType. Tipo di XML Advanced Electronic Signature XAdES"
type: docs
url: /it/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Tipo di firma elettronica avanzata XML (XAdES).

```csharp
public enum XAdESType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | XAdES è disattivato. |
| XAdES | `1` | XAdES di base. |

### Esempi

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
            // Directory di origine
            string sourceDir = "path_to_source_directory";
            // Directory di destinazione
            string outputDir = "path_to_output_directory";
            // Carica la cartella di lavoro
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Definisci la password per il file PFX
            string password = "pfxPassword";
            // Percorso del file PFX
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Crea una firma digitale
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Imposta il tipo XAdES
            signature.XAdESType = XAdESType.XAdES;

            // Crea una collezione di firme digitali
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Imposta la firma digitale nella cartella di lavoro
            workbook.SetDigitalSignature(dsCollection);

            // Salva la cartella di lavoro con la firma digitale
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Verifica la firma digitale
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

### Vedi anche

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


