---
title: "PivotItem.IsFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotItem 属性。指示此数据透视项是否为计算公式项"
type: docs
url: /zh/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

指示此数据透视项是否为计算公式项。

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### 备注

注意：此属性已过时。请改用 PivotItem.IsCalculatedItem 属性。此属性将在自 2024 年 11 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 获取第一个数据透视项
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // 显示当前 IsFormula 值（已过时属性）
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // 为 IsFormula 设置新值（已过时属性）
            pivotItem.IsFormula = true;

            // 演示效果 - 这将把透视项标记为公式项
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // 注意：在实际使用中，您应该改用 IsCalculatedItem，因为 IsFormula 已过时
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // 保存结果
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


