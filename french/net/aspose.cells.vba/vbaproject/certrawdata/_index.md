---
title: "VbaProject.CertRawData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Obtient les données brutes du certificat si ce projet VBA est signé"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Obtient les données brutes du certificat si ce projet VBA est signé.

```csharp
public byte[] CertRawData { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec le projet VBA
            Workbook workbook = new Workbook();
            // Pas besoin de créer un nouveau VbaProject car le classeur en possède déjà un

            // Accéder au projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Vérifier si le projet VBA est signé
            if (vbaProject.IsSigned)
            {
                // Afficher les données brutes du certificat si signé
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Exemple : Enregistrer les données du certificat dans un fichier si elles existent
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // Scénario d'exemple : Charger un classeur avec un projet VBA signé
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // Enregistrez le classeur
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


