---
title: "Range.Transpose"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。Transpose 将数据从行旋转到列或反向旋转"
type: docs
url: /zh/net/aspose.cells/range/transpose/
---
## Range.Transpose method

将数据从行（旋转）到列或反向旋转。

```csharp
public void Transpose()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在 3x3 范围 (A1:C3) 中填充示例数据
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // 创建一个范围 (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // 转置该范围
            range.Transpose();
            
            // 保存工作簿
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### 另请参见

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


