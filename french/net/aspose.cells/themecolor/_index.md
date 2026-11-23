---
title: "Classe ThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ThemeColor. Représente une couleur de thème"
type: docs
url: /fr/net/aspose.cells/themecolor/
---
## ThemeColor class

Représente une couleur de thème.

```csharp
public class ThemeColor
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Obtient et définit le type de thème. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Obtient et définit la valeur de teinte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Ajout d'une valeur à la cellule A1
            cells["A1"].PutValue("Hello World");

            // Obtention du style de la cellule A1
            Style style = cells["A1"].GetStyle();

            // Définir le type de couleur ThemeColorType.Text2 avec un éclaircissement de 40 % comme couleur de police.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Définir le type de couleur ThemeColorType.Background2 avec un assombrissement de 75 % comme couleur de premier plan
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Application du style à la cellule A1
            cells["A1"].SetStyle(style);

            // Enregistrement du fichier Excel
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


