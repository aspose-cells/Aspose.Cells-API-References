---
title: "ExternalConnection.ClassType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExternalConnection property. 获取此 ExternalConnection 对象的类型"
type: docs
url: /zh/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

获取此 [`ExternalConnection`](../) 对象的类型。

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 添加示例数据
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // 使用数据模型连接创建数据透视表
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 获取外部连接并演示 ClassType 属性
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // 保存工作簿
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


