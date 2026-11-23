---
title: "Metered.IsMeteredLicensed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Metered. Vérifie si Metered est licencié"
type: docs
url: /fr/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Vérifiez si Metered est licencié

```csharp
public static bool IsMeteredLicensed()
```

### Valeur de retour

Vrai ou faux

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance Metered
            Metered metered = new Metered();

            try
            {
                // Vérifier si la licence metered est appliquée
                bool isLicensed = Metered.IsMeteredLicensed();

                // Afficher le résultat
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Ajouter le résultat à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


