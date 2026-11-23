---
title: "HtmlTableLoadOption.Name"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOption 属性。获取或设置从 HTML 导入的表格名称"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

获取或设置从 HTML 导入的表格名称

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 按表索引添加新的 HtmlTableLoadOption
            int index = tableLoadOptions.Add(0);

            // 访问 HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // 设置 Name 属性
            option.Name = "CustomerDataTable";

            // 加载 HTML 文件（替换为实际文件路径）
            workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


