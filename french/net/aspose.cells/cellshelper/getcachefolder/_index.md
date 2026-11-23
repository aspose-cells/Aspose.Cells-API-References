---
title: "CellsHelper.GetCacheFolder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données"
type: docs
url: /fr/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

```csharp
public static string GetCacheFolder()
```

### Valeur de retour

Dossier pour les fichiers de cache qui a été spécifié. S'il n'a pas été spécifié, null sera retourné et le chemin temporaire du système sera utilisé si nécessaire.

### Remarques

Les fichiers de cache sont généralement utilisés pour certaines fonctionnalités afin d'optimiser les performances mémoire, comme l'enregistrement d'un grand jeu de données dans un fichier xls, ou l'utilisation du mode mémoire avec cache de fichiers pour le modèle de cellules.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // Obtenir le chemin actuel du dossier de cache
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Afficher le chemin du dossier de cache
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Optionnellement définir un nouveau dossier de cache (démontrant la méthode associée)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Vérifier le changement
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Revenir à l'original (optionnel)
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


