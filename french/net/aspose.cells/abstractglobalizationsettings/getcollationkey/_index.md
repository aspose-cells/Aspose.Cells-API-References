---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractGlobalizationSettings. Transforme la chaîne en un objet comparable selon certaines règles de collation"
type: docs
url: /fr/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Transforme la chaîne en un objet comparable selon certaines règles de collation.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| v | String | La valeur de chaîne doit être comparée avec d'autres. |
| ignoreCase | Boolean | si ignorer la casse lors de la comparaison des valeurs |

### Valeur de retour

L'objet peut être utilisé pour comparer ou trier des valeurs de chaîne

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer des paramètres de mondialisation personnalisés qui remplacent la méthode GetCollationKey
            var settings = new CustomGlobalizationSettings();
            
            // Créer un classeur avec des paramètres de mondialisation personnalisés
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Préparer la chaîne pour la clé de collation
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Appeler GetCollationKey directement
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Démontrer l'effet en l'utilisant dans les opérations de feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Le tri utilisera GetCollationKey en interne
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### Voir aussi

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


