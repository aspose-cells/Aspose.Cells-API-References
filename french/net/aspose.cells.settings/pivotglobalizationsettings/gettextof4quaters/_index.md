---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local des 4 Trimestres"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Obtient le texte local de 4 Trimestres.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetTextOf4Quarters(). Cette propriété sera supprimée 12 mois plus tard à partir de juillet 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une classe de paramètres de mondialisation personnalisée qui hérite de PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Appeler la méthode GetTextOf4Quaters
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Afficher les noms des trimestres dans la console
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Ajouter les noms des trimestres à la feuille de calcul
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Implémentation personnalisée de PivotGlobalizationSettings pour remplacer GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Retourner les noms de trimestre personnalisés
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Voir aussi

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


