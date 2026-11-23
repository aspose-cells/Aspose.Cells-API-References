---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DeleteBlankOptions 属性。指示当单元格是公式且计算结果为 null 或空字符串时是否将其视为空白。默认值为 false"
type: docs
url: /zh/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

当单元格为公式且计算结果为 null 或空字符串时，是否将其视为空白。默认值为 false。

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### 备注

通常情况下，用户应确保在将此属性设为 true 并执行删除操作之前已计算公式。否则，所有通过普通 API（如 [`Formula`](../../cell/formula/)）新创建的公式将被视为空白，并可能被删除，因为在计算之前它们的计算结果都是 null。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // 填充示例数据
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // 删除空白行（不考虑公式空白）
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // 重置数据
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // 删除空白行，将公式空白视为空
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### 另请参见

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


