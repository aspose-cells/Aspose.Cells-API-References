---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. représente le type de mise en forme de l'arrière-plan de page avec image"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Représente le type de mise en forme de l'arrière-plan de la page avec image.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Position | `0` | Définir l'image à une position spécifique. |
| Area | `1` | Étendre l'image. |
| Tile | `2` | Répéter et répéter l'image. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la PageSetup de la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;

            // Accéder à ODSPageBackground du PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Définissez la couleur d'arrière-plan
            odsPageBackground.Color = Color.LightBlue;

            // Définir le type de graphique d'arrière-plan sur Tile
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Définir le chemin du graphique lié (en supposant que l'image se trouve dans le même répertoire que l'exécutable)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Enregistrez le classeur
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


