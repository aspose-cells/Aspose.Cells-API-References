---
title: "AboveAverage.IsAboveAverage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AboveAverage. Obtient ou définit le drapeau indiquant si la règle est une règle au‑dessus de la moyenne. true indique au‑dessus de la moyenne. La valeur par défaut est true."
type: docs
url: /fr/net/aspose.cells/aboveaverage/isaboveaverage/
---
## AboveAverage.IsAboveAverage property

Obtenez ou définissez le drapeau indiquant si la règle est une règle « au‑dessus de la moyenne ». 'true' indique « au‑dessus de la moyenne ». La valeur par défaut est true.

```csharp
public bool IsAboveAverage { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsAboveAverageDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour démontrer la mise en forme conditionnelle
            for (int i = 0; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définir la plage du format conditionnel
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Ajouter une condition AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Configurer les propriétés AboveAverage
            fc.AboveAverage.IsAboveAverage = true;  // Highlight values above average
            fc.AboveAverage.IsEqualAverage = false; // Exclude values equal to average

            // Enregistrez le fichier Excel
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


