---
title: "Workbook.GetDigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Obtient la signature numérique à partir du fichier"
type: docs
url: /fr/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Obtient la signature numérique du fichier.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Appelez la méthode GetDigitalSignature pour récupérer les signatures numériques
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Afficher les informations sur les signatures numériques
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // Enregistrez le classeur
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


