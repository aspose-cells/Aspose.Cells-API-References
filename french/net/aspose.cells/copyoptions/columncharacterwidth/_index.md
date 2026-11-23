---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Indique si la largeur de colonne est copiée en unités de caractères"
type: docs
url: /fr/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Indique si la largeur des colonnes est copiée en unités de caractères.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec des données d'exemple
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Définir la largeur de colonne en caractères pour la démonstration
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Ajoutez des données d'exemple
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copier avec ColumnCharacterWidth défini sur true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Enregistrer le résultat
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Pour comparaison, copier sans ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


