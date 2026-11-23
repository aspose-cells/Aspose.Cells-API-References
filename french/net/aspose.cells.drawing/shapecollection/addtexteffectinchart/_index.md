---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Insère un objet WordArt dans le graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Insère un objet WordArt au graphique.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| effet | MsoPresetTextEffect | Le type d'effet de texte prédéfini mso. |
| texte | String | Le texte WordArt. |
| fontName | String | Le nom de la police. |
| taille | Int32 | La taille de la police |
| fontBold | Boolean | Indique si la police est en gras. |
| fontItalic | Boolean | Indique si la police est en italique. |
| haut | Int32 | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | Int32 | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| hauteur | Int32 | Représente la hauteur de la forme, en unités de 1/4000 de la zone du graphique. |
| largeur | Int32 | Représente la largeur de la forme, en unités de 1/4000 de la zone du graphique. |

### Valeur de retour

Renvoie un objet Shape qui représente le nouvel objet WordArt.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Ajouter du WordArt au graphique
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // Personnaliser l'apparence du WordArt
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Enregistrez le classeur
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


