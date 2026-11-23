---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilterCollection 方法。按数据透视字段的值进行过滤"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

按数据透视字段的值进行过滤。

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baseFieldIndex | Int32 | 源中字段的索引。 |
| valueFieldIndex | Int32 | 数据区域中数据字段的索引。 |
| 类型 | PivotFilterType | 过滤数据的类型。只能是 Count、Sum 和 Percent。 |
| isTop | 布尔 | 指示过滤是来自顶部还是底部 |
| itemCount | Int32 | 项目计数 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // 获取透视过滤器集合
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // 添加 Top10 过滤器 - 按销售额显示前 2 项
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


