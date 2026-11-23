---
title: "Style.IsGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le remplissage de la cellule est un motif dégradé"
type: docs
url: /fr/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Indique si l'ombrage de la cellule est un motif dégradé.

```csharp
public bool IsGradient { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style
            Style style = workbook.CreateStyle();
            
            // Définir l'arrière-plan dégradé
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Appliquer le style à une cellule
            worksheet.Cells["A1"].SetStyle(style);
            
            // Vérifier si le style possède un dégradé
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Afficher le résultat
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Enregistrez le classeur
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


