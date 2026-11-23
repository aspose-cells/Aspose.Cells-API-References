---
title: "Enum FormatConditionValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.FormatConditionValueType. Type de valeur de condition"
type: docs
url: /fr/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Type de valeur de condition.

```csharp
public enum FormatConditionValueType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Formula | `0` | La valeur minimale / médiane / maximale pour le dégradé est déterminée par une formule. |
| Max | `1` | Indique que la valeur maximale de la plage doit être utilisée comme valeur maximale pour le dégradé. |
| Min | `2` | Indique que la valeur minimale de la plage doit être utilisée comme valeur minimale pour le dégradé. |
| Number | `3` | Indique que la valeur minimale / médiane / maximale pour le dégradé est spécifiée par une valeur numérique constante. |
| Percent | `4` | La valeur indique qu'un pourcentage entre les valeurs minimale et maximale de la plage doit être utilisé comme valeur minimale / médiane / maximale pour le dégradé. |
| Percentile | `5` | La valeur indique qu'un classement percentiel dans la plage doit être utilisé comme valeur minimale / médiane / maximale pour le dégradé. |
| AutomaticMax | `6` | Indique que la valeur maximale automatique de la plage doit être utilisée comme valeur maximale automatique pour le dégradé. |
| AutomaticMin | `7` | Indique que la valeur minimale automatique de la plage doit être utilisée comme valeur minimale automatique pour le dégradé. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des conditions de formatage
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Définir les propriétés du jeu d'icônes
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Définir la valeur de la cellule et appliquer le formatage
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Accéder au type de valeur de condition de format
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Afficher les valeurs des conditions du jeu d'icônes
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Enregistrez le classeur
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


