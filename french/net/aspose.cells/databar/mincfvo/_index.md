---
title: "DataBar.MinCfvo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtenir ou définir cet objet de valeur minimale du DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max."
type: docs
url: /fr/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Obtenir ou définir l'objet de valeur minimale de ce DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Obtenez la collection de mise en forme conditionnelle
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // Créer un DataBar avec MinCfvo défini sur le type "Value"
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Définir la plage du DataBar
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Enregistrez le classeur
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


