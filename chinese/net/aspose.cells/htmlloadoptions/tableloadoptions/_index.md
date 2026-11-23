---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlLoadOptions 属性。获取 HtmlTableLoadOptionCollection 实例"
type: docs
url: /zh/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

获取 HtmlTableLoadOptionCollection 实例

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // 按索引添加表加载选项
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // 按 ID 添加表加载选项
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // 使用这些选项加载 HTML 文件
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // 保存输出
            workbook.Save("output.xlsx");
            
            // 清除并添加新的表加载选项
            loadOptions.TableLoadOptions.Clear();
            
            // 添加带有工作表索引映射的表加载选项
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // 添加带有 ID 和工作表映射的表加载选项
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // 使用新选项加载并再次保存
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


