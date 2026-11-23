---
title: "OdsPageBackground.IsLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsPageBackground. Indique s'il s'agit d'un graphique lié"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Indique s'il s'agit d'un graphique lié.

```csharp
public bool IsLink { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Affichez la valeur actuelle de IsLink
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Modifiez les propriétés d'arrière-plan existantes au lieu d'en créer une nouvelle
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Affichez la nouvelle valeur de IsLink
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Enregistrer le résultat
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Voir aussi

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


