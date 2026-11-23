---
title: "DataBar.MaxCfvo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtient ou définit cet objet de valeur maximale des DataBars. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min."
type: docs
url: /fr/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Obtenir ou définir l'objet de valeur maximale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Ajouter une mise en forme conditionnelle de barre de données
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Ajouter une barre de données
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // Définir la valeur MaxCfvo
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Enregistrez le classeur
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


