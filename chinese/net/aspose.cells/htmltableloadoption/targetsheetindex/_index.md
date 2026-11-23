---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOption 属性。获取或设置表格所在工作表的目标索引"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

获取或设置表格所在工作表的目标索引。

```csharp
public int TargetSheetIndex { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // 使用 TargetSheetIndex 配置表格加载选项
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // 添加表格加载选项
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // 使用选项加载 HTML 文件
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
            
            // 验证表格已加载到正确的工作表
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


