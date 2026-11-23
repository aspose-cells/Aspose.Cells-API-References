---
title: "枚举 ErrorCellValueType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.ErrorCellValueType 枚举。表示包含错误的单元格值"
type: docs
url: /zh/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

表示包含错误的单元格值。

```csharp
public enum ErrorCellValueType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Value | `1` | 表示包含 #VALUE! 错误的单元格的值。 |
| Ref | `3` | 表示包含 #REF! 错误的单元格的值。 |
| Name | `4` | 表示包含 #NAME? 错误的单元格的值。 |
| NA | `6` | 表示包含 #N/A 错误的单元格的值。 |
| Blocked | `10` | 表示包含 #BLOCKED! 错误的单元格的值。 |
| Busy | `14` | 表示包含 #BUSY! 错误的单元格的值。 |
| Calc | `13` | 表示包含 #CALC! 错误的单元格的值。 |
| Connect | `9` | 表示包含 #CONNECT! 错误的单元格的值。 |
| Field | `12` | 表示包含 #FIELD! 错误的单元格的值。 |
| Spill | `8` | 表示包含 #SPILL! 错误的单元格的值。 |
| Unknown | `11` | 表示包含 #UNKNOWN! 错误的单元格的值。 |
| TimeOut | `19` | 表示包含 #TIMEOUT! 错误的单元格的值。 |
| External | `18` | 表示包含 #EXTERNAL! 错误的单元格的值。 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置一个会导致溢出错误的公式
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // 计算公式以触发错误
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // 预期的溢出错误
            }
            
            // 获取单元格的富值
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // 检查错误类型
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // 保存工作簿
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


