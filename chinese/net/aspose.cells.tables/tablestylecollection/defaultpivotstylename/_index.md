---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TableStyleCollection 属性。获取和设置透视表的默认样式名称"
type: docs
url: /zh/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

获取和设置透视表的默认样式名称。

```csharp
public string DefaultPivotStyleName { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问表格样式集合
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // 显示默认透视表样式名称
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // 更改默认透视表样式
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // 验证更改
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


