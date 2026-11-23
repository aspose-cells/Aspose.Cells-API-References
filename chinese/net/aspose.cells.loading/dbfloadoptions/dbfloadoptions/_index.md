---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DbfLoadOptions 构造函数。选项"
type: docs
url: /zh/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

这些选项。

```csharp
public DbfLoadOptions()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // 使用 #ctor 方法创建 DbfLoadOptions 实例
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // 使用 DBF 加载选项创建工作簿
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // 访问第一个工作表
                Worksheet worksheet = workbook.Worksheets[0];

                // 显示已加载 DBF 文件中的一些数据
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // 以 Excel 格式保存工作簿
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


