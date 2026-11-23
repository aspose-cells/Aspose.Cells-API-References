---
title: "TextureFill.IsTiling"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Indique si l'image est répétée comme texture"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Indique si l'image est utilisée comme texture en mosaïque.

```csharp
public bool IsTiling { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir les données du graphique
            chart.NSeries.Add("A1:B3", true);
            
            // Définir le remplissage de texture pour la zone du graphique
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // Définir la propriété IsTiling
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Vérifier et afficher la valeur IsTiling
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Enregistrez le classeur
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


