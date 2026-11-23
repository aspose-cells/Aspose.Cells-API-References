---
title: "CellRichValue.ErrorValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellRichValue 属性。获取单元格的错误值类型"
type: docs
url: /zh/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

获取单元格的错误值类型。

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在单元格 A1 中创建溢出错误
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // 计算公式以生成溢出错误
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // 预期的溢出错误
            }
            
            // 从单元格 A1 获取富值
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // 检查并显示错误类型
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


