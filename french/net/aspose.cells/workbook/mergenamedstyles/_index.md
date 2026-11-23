---
title: "Workbook.MergeNamedStyles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Fusionne les styles nommés de l'autre fichier Excel"
type: docs
url: /fr/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Fusionne les styles nommés du autre fichier Excel.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Classeur | L'autre fichier |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Créer le workbook cible (celui qui recevra les styles nommés)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Ajouter des données au workbook cible pour le contexte
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Créer le workbook source (celui qui contient les styles nommés à fusionner)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Ajouter des données au workbook source pour le contexte
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // Fusionner les styles nommés de sourceWorkbook dans targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Enregistrer le workbook résultant
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


