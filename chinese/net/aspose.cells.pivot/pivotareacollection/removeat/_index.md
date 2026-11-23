---
title: "PivotAreaCollection.RemoveAt"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotAreaCollection 方法。移除一个数据透视表条件格式化区域设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareacollection/removeat/
---
## PivotAreaCollection.RemoveAt method

移除一个数据透视表条件格式化区域设置。

```csharp
public void RemoveAt(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 索引 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // 添加数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // 定义要添加到数据透视表区域的单元格区域
            CellArea cellArea1 = new CellArea();
            cellArea1.StartRow = 0;
            cellArea1.StartColumn = 0;
            cellArea1.EndRow = 2;
            cellArea1.EndColumn = 1;

            CellArea cellArea2 = new CellArea();
            cellArea2.StartRow = 1;
            cellArea2.StartColumn = 1;
            cellArea2.EndRow = 3;
            cellArea2.EndColumn = 2;

            // 通过选择区域获取数据透视表区域集合
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
            pivotAreas.Add(cellArea2);

            try
            {
                // 在移除前显示数据透视表区域
                Console.WriteLine("Pivot areas before removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }

                // 使用 Int32 参数调用 RemoveAt 方法
                pivotAreas.RemoveAt(0);

                Console.WriteLine("\nPivot areas after removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // 保存结果
            workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


