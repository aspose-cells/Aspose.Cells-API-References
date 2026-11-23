---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOption 属性。获取或设置要从 html 导入的表格索引"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

获取或设置要从 HTML 导入的表格索引。

```csharp
public int TableIndex { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 使用 TableIndex = 0（第一个表格）配置表格加载选项
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // 添加表格加载选项
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // 加载 HTML 文件（请替换为实际路径）
            workbook = new Workbook("input.html", loadOptions);

            // 另存为 Excel 文件
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


