---
title: "Enum OperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.OperatorType enum. Représente le type d'opérateur du format conditionnel et de la validation des données"
type: docs
url: /fr/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Représente le type d'opérateur du format conditionnel et de la validation des données.

```csharp
public enum OperatorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Between | `0` | Représente l'opérateur Between du format conditionnel et de la validation des données. |
| Equal | `1` | Représente l'opérateur Equal du format conditionnel et de la validation des données. |
| GreaterThan | `2` | Représente l'opérateur GreaterThan du format conditionnel et de la validation des données. |
| GreaterOrEqual | `3` | Représente l'opérateur GreaterOrEqual du format conditionnel et de la validation des données. |
| LessThan | `4` | Représente l'opérateur LessThan du format conditionnel et de la validation des données. |
| LessOrEqual | `5` | Représente l'opérateur LessOrEqual du format conditionnel et de la validation des données. |
| None | `6` | Représente aucune comparaison. |
| NotBetween | `7` | Représente l'opérateur NotBetween du format conditionnel et de la validation des données. |
| NotEqual | `8` | Représente l'opérateur NotEqual du format conditionnel et de la validation des données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un format conditionnel vide
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définir la plage du format conditionnel
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Ajouter une condition avec OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Ajouter une autre condition avec OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Enregistrez le classeur
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


