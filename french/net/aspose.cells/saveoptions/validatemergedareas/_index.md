---
title: "SaveOptions.ValidateMergedAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier"
type: docs
url: /fr/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Indique si la validation des cellules fusionnées doit être effectuée avant d'enregistrer le fichier.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des valeurs et fusionner des cellules
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // Créer des options d'enregistrement avec ValidateMergedAreas défini sur true
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // Enregistrer le classeur avec validation des zones fusionnées
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


