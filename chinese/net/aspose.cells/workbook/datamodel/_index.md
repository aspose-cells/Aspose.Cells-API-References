---
title: "Workbook.DataModel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 属性。获取工作簿中的数据模型"
type: docs
url: /zh/net/aspose.cells/workbook/datamodel/
---
## Workbook.DataModel property

获取工作簿中的数据模型。

```csharp
public DataModel DataModel { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataModelDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 向工作表添加示例数据以创建数据模型
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("DepartmentID");
            sheet1.Cells["B1"].PutValue("DepartmentName");
            sheet1.Cells["A2"].PutValue(1);
            sheet1.Cells["B2"].PutValue("HR");
            sheet1.Cells["A3"].PutValue(2);
            sheet1.Cells["B3"].PutValue("IT");

            Worksheet sheet2 = workbook.Worksheets.Add("Employees");
            sheet2.Cells["A1"].PutValue("EmployeeID");
            sheet2.Cells["B1"].PutValue("EmployeeName");
            sheet2.Cells["C1"].PutValue("DepartmentID");
            sheet2.Cells["A2"].PutValue(101);
            sheet2.Cells["B2"].PutValue("John");
            sheet2.Cells["C2"].PutValue(1);
            sheet2.Cells["A3"].PutValue(102);
            sheet2.Cells["B3"].PutValue("Alice");
            sheet2.Cells["C3"].PutValue(2);

            // 演示 DataModel 属性的用法
            Console.WriteLine("Data Model Relationships:");
            foreach (DataModelRelationship rel in workbook.DataModel.Relationships)
            {
                Console.WriteLine($"Relationship: {rel.PrimaryKeyTable}.{rel.PrimaryKeyColumn} -> {rel.ForeignKeyTable}.{rel.ForeignKeyColumn}");
            }

            Console.WriteLine("\nData Model Tables:");
            foreach (DataModelTable table in workbook.DataModel.Tables)
            {
                Console.WriteLine($"Table: {table.Name}");
            }

            // 保存工作簿
            workbook.Save("WorkbookWithDataModel.xlsx");
        }
    }
}
```

### 另请参见

* class [DataModel](../../../aspose.cells.datamodels/datamodel/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


