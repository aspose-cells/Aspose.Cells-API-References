---
title: "DeleteOptions.UpdateReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteOptions. Indique si les références sont mises à jour dans d'autres feuilles de calcul"
type: docs
url: /fr/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Indique si les références sont mises à jour dans d'autres feuilles de calcul.

```csharp
public bool UpdateReference { get; set; }
```

### Remarques

À partir de la version 26.7, nous définissons la valeur par défaut de cette propriété à true.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et des formules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Créer des options de suppression avec UpdateReference défini sur vrai
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Supprimer la colonne A qui est référencée dans les formules
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


