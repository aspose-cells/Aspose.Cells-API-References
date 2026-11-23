---
title: "Enum DataBarBorderType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DataBarBorderType enum. Spécifie le type de bordure d'une barre de données"
type: docs
url: /fr/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Spécifie le type de bordure d'une barre de données.

```csharp
public enum DataBarBorderType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | La barre de données n'a pas de bordure. |
| Solid | `1` | La barre de données a une bordure solide. |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Ajouter une mise en forme conditionnelle à la feuille de calcul
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Définir une zone de cellules pour la mise en forme conditionnelle
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Ajouter une règle de mise en forme conditionnelle de barre de données
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Accéder à l'objet DataBar
            DataBar dataBar = fc.DataBar;

            // Définir la couleur de la barre de données
            dataBar.Color = Color.Blue;

            // Définir la longueur minimale et maximale de la barre de données
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Définir le type de bordure de la barre de données
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Définir la couleur de la bordure de la barre de données
            dataBar.BarBorder.Color = Color.Red;

            // Enregistrez le classeur
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


