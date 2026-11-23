---
title: "类 HtmlTableLoadOption"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.HtmlTableLoadOption 类。表示从 HTML 导入表格时的选项"
type: docs
url: /zh/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

表示从 HTML 导入表格时的选项。

```csharp
public class HtmlTableLoadOption
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | 获取或设置要从 HTML 导入的表格 ID |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsolete.**) 获取或设置要从 HTML 导入的表格名称 |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | 获取或设置 HTML 中工作表的原始索引。 |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | 获取或设置要从 HTML 导入的表格索引。 |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | 指示是否从导入的表格生成列表对象。默认值为 false。 |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | 获取或设置表格所在工作表的目标索引。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建 HtmlLoadOptions 的实例
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 创建 HtmlTableLoadOption 的实例
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // 将 HtmlTableLoadOption 添加到 HtmlLoadOptions 中
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // 使用指定的加载选项将 HTML 文件加载到工作簿中
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // 将工作簿保存为 Excel 文件
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


