---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TableStyleCollection 属性。获取和设置表格的默认样式名称"
type: docs
url: /zh/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

获取和设置表格的默认样式名称。

```csharp
public string DefaultTableStyleName { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问表格样式集合
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // 显示默认表格样式名称
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // 更改默认表格样式
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


