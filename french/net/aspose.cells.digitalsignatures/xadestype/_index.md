---
title: "Enum XAdESType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.DigitalSignatures.XAdESType. Type de signature électronique avancée XML XAdES"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Type de signature électronique avancée XML (XAdES).

```csharp
public enum XAdESType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | XAdES est désactivé. |
| XAdES | `1` | XAdES de base. |

### Exemples

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
            // Répertoire source
            string sourceDir = "path_to_source_directory";
            // Répertoire de sortie
            string outputDir = "path_to_output_directory";
            // Chargez le classeur
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Définissez le mot de passe pour le fichier PFX
            string password = "pfxPassword";
            // Chemin vers le fichier PFX
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Créez une signature numérique
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Définissez le type XAdES
            signature.XAdESType = XAdESType.XAdES;

            // Créez une collection de signatures numériques
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Attribuez la signature numérique au classeur
            workbook.SetDigitalSignature(dsCollection);

            // Enregistrez le classeur avec la signature numérique
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Vérifiez la signature numérique
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

### Voir aussi

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


