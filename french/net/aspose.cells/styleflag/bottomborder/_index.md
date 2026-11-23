---
title: "StyleFlag.BottomBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Les paramètres de bordure inférieure seront appliqués"
type: docs
url: /fr/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Les paramètres de bordure inférieure seront appliqués.

```csharp
public bool BottomBorder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créer un style avec les paramètres de bordure inférieure
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Créer un indicateur de style et activer la modification de la bordure inférieure
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Appliquer le style avec l'indicateur à la cellule A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
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


