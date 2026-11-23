---
title: "Classe DataBarBorder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DataBarBorder. Représente la bordure des barres de données spécifiées par une règle de mise en forme conditionnelle"
type: docs
url: /fr/net/aspose.cells/databarborder/
---
## DataBarBorder class

Représente la bordure des dataBars spécifiées par une règle de mise en forme conditionnelle.

```csharp
public class DataBarBorder
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Obtient ou définit la couleur de la bordure des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Obtient ou définit le type de la bordure des barres de données spécifiées par une règle de mise en forme conditionnelle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Création d'un nouveau classeur
            Workbook workbook = new Workbook();
            // Accès à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout de données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Ajout d'une mise en forme conditionnelle vide
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définition d'une zone de cellules pour la mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Ajout d'une condition de type DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Accès à la DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Définition des propriétés de la DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Accès et définition des propriétés de DataBarBorder
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Enregistrement du fichier Excel
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


