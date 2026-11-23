---
title: "Top10.IsPercent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Top10. Obtient ou définit si une règle top/bottom n est une règle top/bottom n en pourcentage. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Obtenir ou définir si une règle "top/bottom n" est une règle "top/bottom n percent". La valeur par défaut est false.

```csharp
public bool IsPercent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsPercentDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Ajouter une règle de mise en forme conditionnelle Top10
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);

            // Obtenir la condition de format Top10
            FormatCondition fc = fcc[0];
            
            // Définir les propriétés Top10
            fc.Top10.IsPercent = true;  // Demonstrate IsPercent property
            fc.Top10.IsBottom = false;
            fc.Top10.Rank = 3;

            // Appliquer le style de mise en forme
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Enregistrez le classeur
            workbook.Save("Top10IsPercentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


