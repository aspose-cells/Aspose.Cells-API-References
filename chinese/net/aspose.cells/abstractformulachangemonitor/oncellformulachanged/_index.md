---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractFormulaChangeMonitor 方法。当单元格公式更改时将触发的事件。"
type: docs
url: /zh/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

当单元格中的公式更改时将触发的事件。

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | Int32 | 已更改单元格的工作表索引。 |
| rowIndex | Int32 | 已更改单元格的行索引。 |
| columnIndex | Int32 | 已更改单元格的列索引。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个继承自 AbstractFormulaChangeMonitor 的演示类实例。
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // 在单元格中设置一些公式以触发更改
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // 调用 OnCellFormulaChanged，使用工作表索引 0、行 0、列 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // 处理公式更改的实现
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### 另请参见

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


