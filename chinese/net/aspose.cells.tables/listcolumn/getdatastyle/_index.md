---
title: "ListColumn.GetDataStyle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ListColumn 方法。获取此表格列中数据的样式"
type: docs
url: /zh/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

获取此表格列中数据的样式。

```csharp
public Style GetDataStyle()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向单元格添加示例数据
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // 创建列表对象（表）
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // 从第一列表列获取样式
            Style style = table.ListColumns[0].GetDataStyle();
            
            // 修改样式
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // 将修改后的样式重新应用到列
            table.ListColumns[0].SetDataStyle(style);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


