---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Indique si les lignes et colonnes vides initiales doivent être supprimées comme le fait MS Excel. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait ms excel. La valeur par défaut est true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Remarques

Même règle que dans MS Excel, une ligne/colonne ne sera pas considérée comme vide si elle possède un style personnalisé, même si elle ne contient aucune donnée de cellule. Lors de l'enregistrement en mode LightCells, cette option n'a aucun effet. L'utilisateur doit contrôler la plage de sortie via l'implémentation de [`LightCellsDataProvider`](../lightcellsdataprovider/) ou en spécifiant [`ExportArea`](../exportarea/).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données et des lignes/colonnes vides
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données avec des lignes et colonnes vides initiales
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Enregistrer sans supprimer les espaces vides initiaux
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Enregistrer en supprimant les espaces vides initiaux
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Voir aussi

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


