---
title: "StyleFlag.TopBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure supérieure seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Les paramètres de bordure supérieure seront appliqués.

```csharp
public bool TopBorder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer un style avec les paramètres de bordure supérieure
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Créer un indicateur de style et activer la modification de la bordure supérieure
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Appliquer le style à la cellule A1 avec uniquement l'indicateur de bordure supérieure activé
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(style, styleFlag);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


