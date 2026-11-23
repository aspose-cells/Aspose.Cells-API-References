---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DbfSaveOptions 构造函数。用于保存 .dbf 文件的选项"
type: docs
url: /zh/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

保存 .dbf 文件的选项。

```csharp
public DbfSaveOptions()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // 使用构造函数创建 DbfSaveOptions 实例
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // 设置保存选项的属性
                saveOptions.ExportAsString = true;
                
                // 使用 DBF 保存选项保存工作簿
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


