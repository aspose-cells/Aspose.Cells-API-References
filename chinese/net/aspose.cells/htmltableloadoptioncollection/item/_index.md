---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOptionCollection 属性。获取在指定索引处的 HtmlTableLoadOption 元素"
type: docs
url: /zh/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

获取在指定索引处的 [`HtmlTableLoadOption`](../../htmltableloadoption/) 元素。

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 索引 | 元素的零基索引。 |

### 返回值

指定索引处的元素。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 按表索引添加新的 HtmlTableLoadOption
            int index1 = tableLoadOptions.Add(0);

            // 使用 Item 属性访问 HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // 配置表加载选项
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // 使用已配置的选项加载 HTML 文件
            Workbook workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


