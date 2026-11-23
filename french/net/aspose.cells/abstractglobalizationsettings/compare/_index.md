---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractGlobalizationSettings. Compare deux valeurs de chaîne selon certaines règles de collation"
type: docs
url: /fr/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

Compare deux valeurs de chaîne selon certaines règles de collation.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| v1 | String | la première chaîne |
| v2 | String | la deuxième chaîne |
| ignoreCase | Boolean | si ignorer la casse lors de la comparaison des valeurs |

### Valeur de retour

Entier qui indique la relation lexicale entre les deux comparands

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer des paramètres de mondialisation personnalisés qui remplacent la méthode Compare
            var settings = new CustomGlobalizationSettings();
            
            // Créer un classeur avec des paramètres de mondialisation personnalisés
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Préparer les chaînes à comparer
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // La méthode Compare sera appelée en interne lors d'opérations comme le tri
                // Nous démontrons ici une utilisation directe
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Démontrer l'effet en triant les données
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Créer un DataSorter et définir la plage pour le tri
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### Voir aussi

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


