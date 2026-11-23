---
title: "Validation.GetValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Validation 方法。获取特定单元格上验证的值"
type: docs
url: /zh/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

获取特定单元格上验证的值。

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 行索引。 |
| 列 | Int32 | 列索引。 |
| isValue1 | 布尔 | 指示是否获取第一个值。 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据和验证
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // 为单元格 B1 创建验证
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // 使用 GetValue 方法通过行、列并将数值转换为日期参数获取值
            object value = validation.GetValue(0, 1, false);
            
            // 输出结果
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### 另请参见

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


