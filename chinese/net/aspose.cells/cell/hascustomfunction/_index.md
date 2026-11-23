---
title: "Cell.HasCustomFunction"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Cell 属性。检查此单元格公式中是否存在自定义函数（不受支持的函数）"
type: docs
url: /zh/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

检查此单元格公式中是否存在自定义函数（不受支持的函数）。

```csharp
public bool HasCustomFunction { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook wb = new Workbook();
            
            // 添加自定义函数名称
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // 访问第一个工作表
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // 使用内置函数进行测试
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // 使用自定义函数进行测试
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // 使用包含自定义函数的命名范围进行测试
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // 使用嵌套自定义函数进行测试
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### 另请参见

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


