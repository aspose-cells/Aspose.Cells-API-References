---
title: "类 PivotFieldSortSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting 类。表示用于对数据透视字段进行排序的设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

表示用于对数据透视字段进行排序的设置。

```csharp
public class PivotFieldSortSetting
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | 按行或列中的值进行排序。 |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**已弃用。**) 表示排序字段的索引。-1 表示按标签对 PivotField 排序，其他值表示按数据字段排序。 |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | 指示是否将应用简单的数据排序操作。 |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | 指示是按字段本身还是按数据字段进行排序。 |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | 排序依据的数据透视行类型。 |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | 表示排序字段的索引。-1 表示按数据透视项自身的值排序。当值大于等于零时，表示数据区域中数据字段的索引。 |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | 表示 [`SortOrder`](../../aspose.cells/sortorder/)。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 从数据透视表获取数据透视字段排序设置
            // 注意：此假设数据透视表具有我们可以访问的排序设置
            // 由于我们无法直接创建新的 PivotFieldSortSetting
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // 显示属性（只读）
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // 将排序应用于数据透视表（实际排序将通过数据透视表方法完成）
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // 保存结果
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


