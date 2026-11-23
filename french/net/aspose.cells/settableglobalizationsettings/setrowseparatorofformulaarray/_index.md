---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le séparateur pour les lignes dans les données de tableau d’une formule"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

Définit le séparateur pour les lignes des données de tableau dans la formule.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| c | Char | le séparateur spécifié |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définir le séparateur de ligne pour les tableaux de formules à '|'
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            // Créer une formule de tableau dans la feuille de calcul
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // Calculer la formule pour appliquer les paramètres
                workbook.CalculateFormula();

                // Afficher la formule avec le nouveau séparateur de ligne
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


