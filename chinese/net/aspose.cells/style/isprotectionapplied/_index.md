---
title: "Style.IsProtectionApplied"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Style 属性。指示是否应应用保护格式"
type: docs
url: /zh/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

指示是否应应用保护格式。

```csharp
public bool IsProtectionApplied { get; set; }
```

### 备注

仅适用于已命名的样式。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 创建样式对象
            Style style = workbook.CreateStyle();
            
            // 设置保护属性
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // 将样式应用于单元格
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // 验证保护设置
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // 修改保护设置
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### 另请参见

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


