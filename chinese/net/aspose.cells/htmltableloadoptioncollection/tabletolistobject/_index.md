---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOptionCollection 属性。指示是否从导入的表生成列表对象。默认值为 false。"
type: docs
url: /zh/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

指示是否从导入的表生成列表对象。默认值为 false。

```csharp
public bool TableToListObject { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection 实例
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 设置 TableToListObject 属性以将 HTML 表转换为 ListObjects
            tableLoadOptions.TableToListObject = true;

            // 按索引添加要转换为 ListObject 的表
            tableLoadOptions.Add(0);

            // 使用加载选项将 HTML 文件加载到工作簿中
            workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


