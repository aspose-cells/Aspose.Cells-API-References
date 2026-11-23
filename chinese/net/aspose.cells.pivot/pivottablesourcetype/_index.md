---
title: "枚举 PivotTableSourceType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotTableSourceType 枚举。表示数据透视表的数据源类型。"
type: docs
url: /zh/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

表示数据透视表的数据源类型。

```csharp
public enum PivotTableSourceType : byte
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Sheet | `1` | 指定源数据为一个范围。 |
| External | `2` | 指定使用外部源数据。 |
| Consolidation | `4` | 指定使用多个合并范围作为源数据。 |
| Scenario | `8` | 源数据从临时内部结构中填充。 |
| Unknown | `9` | 未知的数据源。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 向工作表添加示例数据
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // 创建数据透视表集合
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // 使用 Sheet 作为源类型添加数据透视表
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // 显示源类型
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // 演示不同的源类型
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // 保存工作簿
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


