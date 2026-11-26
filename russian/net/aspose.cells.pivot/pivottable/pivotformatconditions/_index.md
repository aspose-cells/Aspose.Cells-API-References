---
title: "PivotTable.PivotFormatConditions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает условия форматирования сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/pivotformatconditions/
---
## PivotTable.PivotFormatConditions property

Получает условия форматирования сводной таблицы.

```csharp
[Obsolete("Use PivotTable.ConditionalFormats property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFormatConditionCollection PivotFormatConditions { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotTable.ConditionalFormats. Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotFormatConditionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Добавьте примерные данные
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Year";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Laptop";
            cells["A3"].Value = "Phone";
            cells["A4"].Value = "Tablet";
            cells["A5"].Value = "Laptop";
            cells["A6"].Value = "Phone";
            cells["A7"].Value = "Tablet";

            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2021;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;

            cells["C2"].Value = 1500;
            cells["C3"].Value = 800;
            cells["C4"].Value = 400;
            cells["C5"].Value = 1800;
            cells["C6"].Value = 950;
            cells["C7"].Value = 500;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "SalesPivot");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Year");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить условие форматирования
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = fcc[conditionIndex];
            condition.Formula1 = "1000";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.LightGreen;

            pfc.ScopeType = PivotConditionFormatScopeType.Data;

            // Обновить и сохранить
            pivot.RefreshData();
            workbook.Save("PivotTableFormatConditionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFormatConditionCollection](../../pivotformatconditioncollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


