---
title: "PivotField.SortSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。获取自动排序的所有设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/sortsetting/
---
## PivotField.SortSetting property

获取自动排序的所有设置

```csharp
public PivotFieldSortSetting SortSetting { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertySortSettingDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 75;

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];

            // 演示 SortSetting 属性
            rowField.SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + rowField.SortSetting.Cell);
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);

            // 更改排序设置
            rowField.SortBy(SortOrder.Descending, 0, PivotLineType.GrandTotal, null);
            Console.WriteLine("\nAfter changing sort settings:");
            Console.WriteLine("Sort Type: " + rowField.SortSetting.SortType);
            Console.WriteLine("Sorted by Cell: " + (string.IsNullOrEmpty(rowField.SortSetting.Cell) ? "null" : rowField.SortSetting.Cell));
            Console.WriteLine("Line Type Sorted By: " + rowField.SortSetting.LineTypeSortedBy);
        }
    }
}
```

### 另请参见

* class [PivotFieldSortSetting](../../pivotfieldsortsetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


