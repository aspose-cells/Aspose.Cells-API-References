---
title: "Classe Top10"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Top10. Décrivez la règle de mise en forme conditionnelle Top10. Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans la tranche supérieure N ou inférieure N spécifiée."
type: docs
url: /fr/net/aspose.cells/top10/
---
## Top10 class

Décrit la règle de mise en forme conditionnelle Top10. Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans la tranche supérieure N ou inférieure N, selon la spécification.

```csharp
public class Top10
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Top10](top10/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Obtenir ou définir si une règle "top/bottom n" est une règle "bottom n". La valeur par défaut est false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Obtenir ou définir si une règle "top/bottom n" est une règle "top/bottom n percent". La valeur par défaut est false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Obtenir ou définir la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est true, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. La valeur par défaut est 10. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Ajoute une condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Définition des propriétés
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Enregistrement du fichier Excel
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


