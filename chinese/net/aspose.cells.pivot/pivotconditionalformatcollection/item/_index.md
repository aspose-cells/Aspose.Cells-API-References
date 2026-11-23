---
title: "PivotConditionalFormatCollection.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotConditionalFormatCollection 属性。 获取特定索引处的枢轴 FormatCondition 对象"
type: docs
url: /zh/net/aspose.cells.pivot/pivotconditionalformatcollection/item/
---
## PivotConditionalFormatCollection indexer

获取特定索引处的透视 FormatCondition 对象。

```csharp
public PivotConditionalFormat this[int index] { get; }
```

### 返回值

枢轴 FormatCondition 对象。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 120;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 85;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 95;

            // 创建数据透视表
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 添加条件格式
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex]; // Using Item property
            pfc.AddCellArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 10, EndColumn = 10 });

            // 添加格式条件
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "90";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.LightGreen;

            // 计算枢轴表并保存
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotConditionalFormat](../../pivotconditionalformat/)
* class [PivotConditionalFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


