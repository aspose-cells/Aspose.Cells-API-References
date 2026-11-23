---
title: "ExportTableOptions.AllowDBNull"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExportTableOptions 属性。此值指示是否在此表中允许 DBNull"
type: docs
url: /zh/net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

此值指示是否在此表中允许 DBNull。

```csharp
public bool AllowDBNull { get; set; }
```

### 示例

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyAllowDBNullDemo
    {
        public static void Run()
        {
            // 创建一个带有测试数据的示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加包含一些空单元格的示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue(""); // Empty cell
            worksheet.Cells["B3"].PutValue(25);

            // 导出时 AllowDBNull = true（默认）
            ExportTableOptions options1 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = true
            };
            
            DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
            Console.WriteLine("With AllowDBNull=true:");
            Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));

            // 导出时 AllowDBNull = false
            ExportTableOptions options2 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = false
            };
            
            DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
            Console.WriteLine("\nWith AllowDBNull=false:");
            Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
        }
    }
}
```

### 另请参见

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


