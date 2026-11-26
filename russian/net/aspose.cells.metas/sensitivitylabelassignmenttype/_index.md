---
title: "Перечисление SensitivityLabelAssignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Metas.SensitivityLabelAssignmentType enum. Представляет метод назначения метки конфиденциальности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabelassignmenttype/
---
## SensitivityLabelAssignmentType enumeration

Представляет метод назначения метки чувствительности.

```csharp
public enum SensitivityLabelAssignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Standard | `0` | Используйте для любой метки конфиденциальности, которая не была применена пользователем напрямую. |
| Privileged | `1` | Используйте для любой метки конфиденциальности, которая была применена пользователем напрямую. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;

    public class MetasClassSensitivityLabelAssignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрировать значения перечисления SensitivityLabelAssignmentType
            SensitivityLabelAssignmentType standardAssignment = SensitivityLabelAssignmentType.Standard;
            SensitivityLabelAssignmentType privilegedAssignment = SensitivityLabelAssignmentType.Privileged;

            // Применить тип назначения метки конфиденциальности к метаданным листа
            worksheet.Cells["A1"].PutValue("Standard Sensitivity Label Assignment:");
            worksheet.Cells["B1"].PutValue(standardAssignment.ToString());

            worksheet.Cells["A2"].PutValue("Privileged Sensitivity Label Assignment:");
            worksheet.Cells["B2"].PutValue(privilegedAssignment.ToString());

            // Условное форматирование на основе типа назначения метки конфиденциальности
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

            // Сохраните книгу
            workbook.Save("SensitivityLabelAssignmentTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


