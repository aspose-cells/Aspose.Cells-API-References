---
title: "PivotAreaCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotAreaCollection. Возвращает объект PivotArea"
type: docs
url: /ru/net/aspose.cells.pivot/pivotareacollection/item/
---
## PivotAreaCollection indexer

Возвращает объект [`PivotArea`](../../pivotarea/);

```csharp
public PivotArea this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;

            // Создать сводную таблицу
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Добавить условный формат
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            pfc.AddCellArea(CellArea.CreateCellArea("A5", "B8"));

            // Доступ к PivotAreas с помощью свойства Item
            PivotArea pivotArea = pfc.PivotAreas[0]; // Using Item indexer
            pivotArea.RuleType = PivotAreaType.All;

            // Добавить условие форматирования
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "150";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = Color.Red;

            // Выполнить расчёт и сохранить
            pivot.CalculateData();
            workbook.Save("PivotAreaCollectionPropertyItemDemo_output.xlsx");
        }
    }
}
```

### См. также

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


