---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir la feuille de calcul avec des données incluant des chaînes vides
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Configurer DeleteBlankOptions avec EmptyStringAsBlank défini sur true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Supprimer les lignes contenant des chaînes vides (traitées comme vides)
            worksheet.Cells.DeleteBlankRows(options);

            // Enregistrer le résultat
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


