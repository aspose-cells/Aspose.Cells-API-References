---
title: "StyleFlag.ShrinkToFit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre Réduire pour ajuster sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Le paramètre de réduction pour ajuster sera appliqué.

```csharp
public bool ShrinkToFit { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir des données d'exemple dans une cellule
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Créer un style avec ShrinkToFit activé
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Créer un indicateur de style et activer l'indicateur ShrinkToFit
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Appliquer le style à la plage de cellules (en utilisant explicitement Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Définir la largeur de colonne pour démontrer le rétrécissement
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Enregistrez le classeur
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


