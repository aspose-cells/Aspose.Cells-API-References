---
title: "PasteOptions.KeepOldTables"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PasteOptions 属性。保留目标范围中的表格"
type: docs
url: /zh/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

保留目标范围内的表格。

```csharp
public bool KeepOldTables { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建带有数据的示例工作表
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // 创建一个 PasteOptions 实例
                PasteOptions pasteOptions = new PasteOptions();

                // 显示 KeepOldTables 属性的默认值
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // 将 KeepOldTables 设置为 true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // 为复制操作创建范围
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // 使用 KeepOldTables 选项进行复制
                targetRange.Copy(sourceRange, pasteOptions);

                // 保存工作簿
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


