---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeProtectionProvider. Obtient le mot de passe pour protéger la feuille de calcul spécifiée"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Obtient le mot de passe pour protéger la feuille de calcul spécifiée.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Valeur de retour

Mot de passe pour protéger la feuille de calcul spécifiée.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Créez une instance de fournisseur de protection personnalisé
            var provider = new CustomProtectionProvider();

            try
            {
                // Appeler GetWorksheetPassword avec le nom de la feuille de calcul
                string password = provider.GetWorksheetPassword(sheetName);

                // Appliquer la protection à la feuille de calcul en utilisant le mot de passe récupéré
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Enregistrez le classeur protégé
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Implémentation personnalisée renvoyant le mot de passe basé sur le nom de la feuille
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Logique simple de génération de mot de passe à des fins de démonstration
            return $"pw_{sheetName}";
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


