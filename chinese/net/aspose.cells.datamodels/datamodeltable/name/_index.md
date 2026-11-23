---
title: "DataModelTable 属性。获取数据模型表的连接名称"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "显示当前 ConnectionName 值"
type: docs
url: /zh/net/aspose.cells.datamodels/datamodeltable/name/
---
## DataModelTable.Name property

获取数据模型表的名称。

```csharp
public string Name { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            DataModel dataModel = workbook.DataModel;
            if (dataModel.Tables.Count == 0)
            {
                Console.WriteLine("Workbook data model contains no tables. Add tables to the data model first.");
                return;
            }

            DataModelTable table = dataModel.Tables[0];
            Console.WriteLine("Current DataModelTable Name: " + table.Name);
            
            Worksheet sheet = workbook.Worksheets.Add("Report");
            int pivotIndex = sheet.PivotTables.Add("PivotTable1", "A1", table.Name);
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            workbook.Save("DataModelTableNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


