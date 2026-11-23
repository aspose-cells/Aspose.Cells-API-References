---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookDesigner 方法。将 json 字符串值设为智能标记的数据源"
type: docs
url: /zh/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

将 json 字符串值设为智能标记的数据源。

```csharp
public void SetJsonDataSource(string name, string json)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | String | 表的名称。如果 JSON 的值表示一个对象，则可能为 null。 |
| json | String | Json 字符串的值。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 在单元格 A1 中添加示例标记
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // 创建工作簿设计器
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // 示例 JSON 数据
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // 设置 JSON 数据源
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // 处理标记
            designer.Process();
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


