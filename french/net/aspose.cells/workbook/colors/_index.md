---
title: "Workbook.Colors"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Retourne les couleurs de la palette pour la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Renvoie les couleurs de la palette pour la feuille de calcul.

```csharp
public Color[] Colors { get; }
```

### Remarques

La palette comporte 56 entrées, chacune représentée par une valeur RVB.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la palette de couleurs par défaut
            Color[] colors = workbook.Colors;

            // Modifier certaines couleurs de la palette
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Créez une feuille de calcul et ajoutez des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Appliquer les couleurs modifiées aux cellules
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Enregistrez le classeur
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


