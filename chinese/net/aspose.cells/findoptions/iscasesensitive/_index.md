---
title: "FindOptions.IsCaseSensitive"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FindOptions 属性。指示搜索的字符串是否区分大小写"
type: docs
url: /zh/net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

指示搜索的字符串是否区分大小写。

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### 备注

注意：此成员已过时。请改用 FindOptions.CaseSensitive 属性。该属性将在自 2010 年 6 月起 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyIsCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置示例数据
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("AbC");

            FindOptions options = new FindOptions();
            options.IsCaseSensitive = true;
            
            // 查找区分大小写的匹配
            Cell cell = worksheet.Cells.Find("abc", null, options);
            
            Console.WriteLine("Case-sensitive search for 'abc' found at: " + 
                              (cell != null ? cell.Name : "No match"));
        }
    }
}
```

### 另请参见

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


