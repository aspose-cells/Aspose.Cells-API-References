---
title: "Enum OdsPageBackgroundType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Ods.OdsPageBackgroundType. Représente le type d'arrière-plan de page du ods"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Représente le type d'arrière-plan de page d'ods.

```csharp
public enum OdsPageBackgroundType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas d'arrière-plan. |
| Color | `1` | Formate l'arrière-plan avec une couleur. |
| Graphic | `2` | Formate l'arrière-plan avec une image. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la PageSetup de la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;

            // Accédez à la propriété ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Définissez le type d'arrière-plan sur Couleur
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Définissez la couleur d'arrière-plan
            odsPageBackground.Color = Color.LightBlue;

            // Enregistrez le classeur
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


