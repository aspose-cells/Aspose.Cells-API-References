---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFieldSortSetting 属性。指示是按字段本身还是按数据字段进行排序"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

指示是按字段本身还是按数据字段进行排序。

```csharp
public bool IsSortByLabels { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // 获取透视字段排序设置
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // 显示当前 IsSortByLabels 值
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // 注意：IsSortByLabels 是只读的，所以我们不能直接设置它
            // 相反，我们将通过检查排序设置来演示其含义

            // 显示相关的排序属性
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // 保存工作簿
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


