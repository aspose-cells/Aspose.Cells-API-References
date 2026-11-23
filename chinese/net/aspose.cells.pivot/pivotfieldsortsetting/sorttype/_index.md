---
title: "PivotFieldSortSetting.SortType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFieldSortSetting 属性。表示 SortOrder"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldsortsetting/sorttype/
---
## PivotFieldSortSetting.SortType property

表示 [`SortOrder`](../../../aspose.cells/sortorder/)。

```csharp
public SortOrder SortType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertySortTypeDemo
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
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // 按升序对行字段进行排序
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E5");
            
            // 演示 SortType 属性
            Console.WriteLine("Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
            
            // 更改排序顺序并再次演示
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "E6");
            Console.WriteLine("Updated Sort Type: " + pivotTable.RowFields[0].SortSetting.SortType);
            Console.WriteLine("Updated sorted by cell: " + pivotTable.RowFields[0].SortSetting.Cell);
        }
    }
}
```

### 另请参见

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


