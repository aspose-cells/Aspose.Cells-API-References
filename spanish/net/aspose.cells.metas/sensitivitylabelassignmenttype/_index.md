---
title: "Enumeración SensitivityLabelAssignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Representa el método de asignación para la etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabelassignmenttype/
---
## SensitivityLabelAssignmentType enumeration

Representa el método de asignación para la etiqueta de sensibilidad.

```csharp
public enum SensitivityLabelAssignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Standard | `0` | Utilice cualquier etiqueta de sensibilidad que no haya sido aplicada directamente por el usuario. |
| Privileged | `1` | Utilice cualquier etiqueta de sensibilidad que haya sido aplicada directamente por el usuario. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;

    public class MetasClassSensitivityLabelAssignmentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar los valores del enum SensitivityLabelAssignmentType
            SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
            SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;

            // Aplicar el tipo de asignación de etiqueta de sensibilidad a los metadatos de la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
            worksheet.Cells["B1"].PutValue(standardAssignment.ToString());

            worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
            worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());

            // Formato condicional basado en el tipo de asignación de etiqueta de sensibilidad
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

            // Guarda el libro de trabajo
            workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


