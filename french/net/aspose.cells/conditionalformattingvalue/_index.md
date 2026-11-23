---
title: "Classe ConditionalFormattingValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ConditionalFormattingValue. Décrit les valeurs des points d'interpolation dans une barre de données à échelle graduée ou un jeu d'icônes"
type: docs
url: /fr/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Décrit les valeurs des points d'interpolation dans une échelle graduée, une dataBar ou un iconSet.

```csharp
public class ConditionalFormattingValue
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Obtenez ou définissez le drapeau Greater Than Or Equal. Utilisez uniquement pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'greater than' est utilisé au lieu de 'greater than or equal to'. La valeur par défaut est true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Obtenez ou définissez le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement "Value" à null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Obtenez ou définissez la valeur de cet objet de valeur de mise en forme conditionnelle. Elle doit être utilisée conjointement avec Type. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Ajoute une condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Définition des propriétés pour ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Définition de la valeur minimale
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Définition de la valeur médiane
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Définition de la valeur maximale
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Enregistrez le classeur
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


