---
title: "Range.IsBlank"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。指示该范围是否包含值"
type: docs
url: /zh/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

指示该范围是否包含值。

```csharp
public bool IsBlank()
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 创建一个范围并检查它是否为空（应为 true）
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // 在一个单元格中放入一个值后再次检查（应为 false）
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### 另请参见

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


