---
title: "ListObject.HasAutoFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ListObject 属性。指示是否对该表应用了自动筛选"
type: docs
url: /zh/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

指示是否对该表应用了自动筛选。

```csharp
public bool HasAutoFilter { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为表填充示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // 添加覆盖数据范围的 ListObject（表）
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // 确保表已调整大小以包含所有行
                listObject.Resize(0, 0, 4, 2, true);

                // 读取并显示 HasAutoFilter 属性值
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // 可以通过 AutoFilter 属性访问 AutoFilter 对象
                // 演示当 HasAutoFilter 为 true 时它不为 null
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // 在 "Score" 列（索引 1）上应用一个简单过滤器，以显示 Score >= 80 的行
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // 使用 Cells.Rows 检查该行是否被隐藏
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // 清除过滤器
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // 保存工作簿（可选）
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


