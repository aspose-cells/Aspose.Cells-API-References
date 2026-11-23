---
title: "IFilePathProvider.GetFullName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IFilePathProvider. Obtient le chemin complet du fichier par le nom de la Worksheet lors de l'exportation de la Worksheet vers HTML séparément. Ainsi, les références entre les Worksheets peuvent être exportées correctement"
type: docs
url: /fr/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Obtient le chemin complet du fichier par le nom de la feuille de calcul lors de l'exportation de la feuille de calcul en HTML séparément. Ainsi, les références entre les feuilles de calcul peuvent être exportées correctement.

```csharp
public string GetFullName(string sheetName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | String | Nom de la feuille de calcul |

### Valeur de retour

le chemin complet du fichier

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Créez une implémentation personnalisée de IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Appelez la méthode GetFullName avec le nom d'une feuille
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Afficher le résultat
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Implémentation simple qui retourne un chemin combinant le nom de la feuille avec un répertoire
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Voir aussi

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


