---
title: "Enum SensitivityLabelAssignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Rappresenta il metodo di assegnazione per l'etichetta di sensibilità"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabelassignmenttype/
---
## SensitivityLabelAssignmentType enumeration

Rappresenta il metodo di assegnazione per l'etichetta di sensibilità.

```csharp
public enum SensitivityLabelAssignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Standard | `0` | Usa per qualsiasi etichetta di sensibilità che non è stata applicata direttamente dall'utente. |
| Privileged | `1` | Usa per qualsiasi etichetta di sensibilità che è stata applicata direttamente dall'utente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;

    public class MetasClassSensitivityLabelAssignmentTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra i valori dell'enum SensitivityLabelAssignmentType
            SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
            SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;

            // Applica il tipo di assegnazione dell'etichetta di sensibilità ai metadati del foglio di lavoro
            worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
            worksheet.Cells["B1"].PutValue(standardAssignment.ToString());

            worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
            worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());

            // Formattazione condizionale basata sul tipo di assegnazione dell'etichetta di sensibilità
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

            // Salva la cartella di lavoro
            workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


