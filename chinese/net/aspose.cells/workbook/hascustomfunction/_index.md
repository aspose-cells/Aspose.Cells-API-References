---
title: "Workbook.HasCustomFunction"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 属性。检测工作簿中是否使用了自定义函数，例如在已定义名称的单元格公式中"
type: docs
url: /zh/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

检测工作簿中是否使用了自定义函数，例如在单元格公式或已定义名称中……

```csharp
public bool HasCustomFunction { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook wb = new Workbook();
            
            // 向名称添加标准公式
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // 向名称添加自定义函数
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // 使用单元格公式进行测试
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // 单元格中的标准函数
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // 单元格中的自定义函数
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // 对包含自定义函数的名称的引用
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // 组合自定义函数
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### 另请参见

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


