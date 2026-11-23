---
title: "HtmlTableLoadOption.Id"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOption 属性。获取或设置从 HTML 导入的表格 id"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

获取或设置要从 HTML 导入的表格 ID

```csharp
public string Id { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // 配置表格加载选项
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // 添加表格加载选项
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // 使用指定选项加载 HTML 文件
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


