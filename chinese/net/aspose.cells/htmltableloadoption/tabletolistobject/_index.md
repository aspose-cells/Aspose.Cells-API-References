---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOption 属性。指示是否从导入的表格生成列表对象。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

指示是否从导入的表格生成列表对象。默认值为 false。

```csharp
public bool TableToListObject { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建启用 TableToListObject 的 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // 使用指定的选项加载 HTML
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


