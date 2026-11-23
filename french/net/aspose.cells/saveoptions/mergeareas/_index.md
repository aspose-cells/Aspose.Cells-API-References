---
title: "SaveOptions.MergeAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique si les zones de mise en forme conditionnelle et de validation doivent être fusionnées avant d'enregistrer le fichier"
type: docs
url: /fr/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant l'enregistrement du fichier.

```csharp
public bool MergeAreas { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données et créer des cellules fusionnées
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Fusionner les cellules A1:B1
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Créer des options d'enregistrement avec MergeAreas activé
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Enregistrer avec l'optimisation des zones fusionnées
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


