---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HighlightChangesOptions 构造函数。表示用于突出显示共享 Excel 文件的修订或更改的选项"
type: docs
url: /zh/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

表示对共享 Excel 文件的修订或更改进行高亮显示的选项。

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| highlightOnScreen | 布尔 | 指示是否在屏幕上突出显示更改。 |
| listOnNewSheet | 布尔 | 指示是否在新工作表上列出更改。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加一些示例数据
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // 使用布尔参数创建 HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // 模拟跟踪更改（通常您会有实际的修订）
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // 保存工作簿
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


