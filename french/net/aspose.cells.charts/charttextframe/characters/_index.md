---
title: "ChartTextFrame.Characters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartTextFrame. Retourne un objet Characters qui représente une plage de caractères dans le texte"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Renvoie un objet Characters qui représente une plage de caractères dans le texte.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index du début du caractère. |
| longueur | Int32 | Le nombre de caractères. |

### Valeur de retour

Objet Characters.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Accéder aux étiquettes de données et définir la taille de police pour des caractères spécifiques
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


