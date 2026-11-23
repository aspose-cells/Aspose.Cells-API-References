---
title: "Énum SensitivityLabelAssignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Représente la méthode d'attribution pour le label de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabelassignmenttype/
---
## SensitivityLabelAssignmentType enumeration

Représente la méthode d'attribution de l'étiquette de sensibilité.

```csharp
public enum SensitivityLabelAssignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Standard | `0` | Utilisez pour tout label de sensibilité qui n'a pas été appliqué directement par l'utilisateur. |
| Privileged | `1` | Utilisez pour tout label de sensibilité qui a été appliqué directement par l'utilisateur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;

    public class MetasClassSensitivityLabelAssignmentTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrez les valeurs de l'énum SensitivityLabelAssignmentType
            SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
            SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;

            // Appliquez le type d'attribution du label de sensibilité aux métadonnées de la feuille de calcul
            worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
            worksheet.Cells["B1"].PutValue(standardAssignment.ToString());

            worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
            worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());

            // Mise en forme conditionnelle basée sur le type d'attribution du label de sensibilité
            int standardLabelIndex = (int)SensitivityLabelAssignmentType.Standard;
            int privilegedLabelIndex = (int)SensitivityLabelAssignmentType.Privileged;

            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            CellArea cellArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };
            int index = formatConditions.AddCondition(FormatConditionType.Expression, OperatorType.None, "", "");
            FormatCondition formatCondition = formatConditions[index];
            formatCondition.SetFormulas("=$B$1=\"" + standardAssignment.ToString() + "\"", "", false, false);
            formatCondition.Type = FormatConditionType.Expression;
            formatCondition.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            index = formatConditions.AddCondition(FormatConditionType.Expression, OperatorType.None, "", "");
            formatCondition = formatConditions[index];
            formatCondition.SetFormulas("=$B$2=\"" + privilegedAssignment.ToString() + "\"", "", false, false);
            formatCondition.Type = FormatConditionType.Expression;
            formatCondition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // Enregistrez le classeur
            workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


