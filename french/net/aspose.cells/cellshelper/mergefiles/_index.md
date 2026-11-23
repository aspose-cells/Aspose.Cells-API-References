---
title: "CellsHelper.MergeFiles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Fusionne plusieurs gros fichiers xls en un fichier xls"
type: docs
url: /fr/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Fusionne plusieurs gros fichiers xls en un fichier xls.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fichiers | String[] | Les fichiers. |
| cachedFile | String | Le fichier en cache. |
| destFile | String | Le fichier de destination. |

### Remarques

Cette méthode ne prend en charge que la fusion des données, du style et des formules dans le nouveau fichier. Le fichier en cache est utilisé pour stocker des données temporaires.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // Créer des fichiers Excel temporaires à fusionner
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Créer des classeurs d'exemple
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // Appeler MergeFiles avec les paramètres String[], String, String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Vérifier le fichier fusionné
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // Nettoyez les fichiers temporaires
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


