---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom de feuille par défaut pour l’ajout automatique d’une feuille de calcul. La valeur par défaut est Sheet"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Obtient le nom de feuille par défaut pour l’ajout automatique d’une feuille de calcul. La valeur par défaut est "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Valeur de retour

le nom de feuille par défaut pour l’ajout automatique d’une feuille de calcul

### Remarques

Le nom de la feuille ajoutée automatiquement (par exemple via [`Add`](../../worksheetcollection/add/)) sera le nom spécifié suivi d’un numéro de séquence. Par exemple, un utilisateur allemand pourrait vouloir que le nom de la feuille soit "Tabellenblatt2" au lieu de "Sheet2". L’utilisateur peut alors implémenter cette méthode pour renvoyer "Tabellenblatt".

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir des paramètres de globalisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Obtenir le nom de feuille par défaut à partir des paramètres de globalisation personnalisés
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Ajouter une nouvelle feuille de calcul pour démontrer la dénomination basée sur la valeur par défaut personnalisée
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Implémentation des paramètres de globalisation personnalisés
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


