---
title: "FindOptions.SearchOrderByRows"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FindOptions 属性。指示搜索顺序是按行还是按列"
type: docs
url: /zh/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

指示搜索顺序是按行还是按列。

```csharp
public bool SearchOrderByRows { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // 创建工作簿并添加示例数据
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 用测试数据填充单元格（在列主序中搜索 "abc"）
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // 创建查找选项并将搜索顺序设置为列主序
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // 查找 "abc" - 在列主序搜索时应返回 A3（第2行，第0列）
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // 输出结果
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### 另请参见

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


