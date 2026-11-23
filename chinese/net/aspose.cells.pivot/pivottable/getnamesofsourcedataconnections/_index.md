---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotTable 方法。获取外部源数据连接的名称"
type: docs
url: /zh/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

获取外部源数据连接的名称。

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 添加示例数据
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // 创建数据透视表并获取引用
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // 获取源数据连接
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // 输出连接信息
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### 另请参见

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


