---
title: "Enum SensitivityLabelAssignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Representerar tilldelningsmetoden för känslighetsetiketten"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabelassignmenttype/
---
## SensitivityLabelAssignmentType enumeration

Representerar tilldelningsmetoden för känslighetsetiketten.

```csharp
public enum SensitivityLabelAssignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Standard | `0` | Använd för alla känslighetsetiketter som inte applicerades direkt av användaren. |
| Privileged | `1` | Använd för alla känslighetsetiketter som applicerades direkt av användaren. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;

    public class MetasClassSensitivityLabelAssignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrera värden för SensitivityLabelAssignmentType-enum
            SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
            SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;

            // Applicera känslighetsetikettens tilldelningstyp på arbetsbladets metadata
            worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
            worksheet.Cells["B1"].PutValue(standardAssignment.ToString());

            worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
            worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());

            // Villkorsstyrd formatering baserad på känslighetsetikettens tilldelningstyp
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

            // Spara arbetsboken
            workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


