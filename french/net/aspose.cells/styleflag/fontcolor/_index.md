---
title: "StyleFlag.FontColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "StyleFlag propriété. Le paramètre de couleur de police sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Le paramètre de couleur de police sera appliqué.

```csharp
public bool FontColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style personnalisé
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Créer un indicateur de style et activer la couleur de police et l'ombrage de cellule
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Appliquer le style à la cellule A1 avec les indicateurs spécifiés
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
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


