---
title: "DataBar.Direction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtient ou définit la direction dans laquelle le DataBar est affiché"
type: docs
url: /fr/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Obtient ou définit la direction dans laquelle le DataBar est affiché.

```csharp
public TextDirectionType Direction { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour démontrer les barres de données
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Ajouter une mise en forme conditionnelle de barre de données
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Définir la zone de cellules pour la condition de formatage
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // Ajouter la condition DataBar et obtenir la référence
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Afficher la valeur actuelle de Direction
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Modifier la direction en RightToLeft et démontrer
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Configuration supplémentaire pour une meilleure visualisation
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Enregistrer le classeur pour montrer l'effet
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


