---
title: "Classe OdsPageBackground"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "classe Aspose.Cells.Ods.OdsPageBackground. Représente l'arrière-plan de la page ODS"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Représente l'arrière-plan de page d'ods.

```csharp
public class OdsPageBackground
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Obtient et définit la couleur de l'arrière-plan. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Obtient et définit les données graphiques. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Obtient et définit la position du graphique d'arrière-plan. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Obtient et définit le type de graphique d'arrière-plan de la page. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Indique s'il s'agit d'un graphique lié. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Obtient et définit le chemin du graphique lié. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Obtient et définit le type d'arrière-plan de la page. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accéder à l'objet PageSetup
            PageSetup pageSetup = sheet.PageSetup;

            // Accédez à l'objet ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Définissez le type d'arrière-plan sur Couleur
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Définissez la couleur d'arrière-plan
            odsPageBackground.Color = Color.LightBlue;

            // Définissez le type de graphique d'arrière-plan
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Définissez la position du graphique d'arrière-plan
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Définissez le chemin du graphique lié (le cas échéant)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Enregistrez le classeur
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


