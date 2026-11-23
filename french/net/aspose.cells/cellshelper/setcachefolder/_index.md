---
title: "CellsHelper.SetCacheFolder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données"
type: docs
url: /fr/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

```csharp
public static void SetCacheFolder(string cache)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cache | String | Dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |

### Remarques

Les fichiers de cache sont généralement utilisés pour certaines fonctionnalités afin d'optimiser les performances mémoire, comme l'enregistrement d'un grand jeu de données dans un fichier xls, ou l'utilisation du mode mémoire avec cache de fichiers pour le modèle de cellules.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un répertoire temporaire pour le cache
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Définir le dossier de cache en utilisant CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Vérifier que le dossier de cache a été défini
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Créer un classeur simple pour démontrer la fonctionnalité
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Enregistrez le classeur
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


