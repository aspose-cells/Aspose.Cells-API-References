---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ExportTableOptions 方法。预处理要导出的当前单元格的值"
type: docs
url: /zh/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

预处理要导出的当前单元格的值。

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellRow | Int32 | 当前单元格的行索引 |
| cellColumn | Int32 | 单元格的列索引 |
| 值 | CellValue | 当前单元格的值和类型 |

### 返回值

当前单元格是否已被替换为不同的类型和/或值。

### 备注

行和列索引是单元格在工作表中的绝对索引，而不是导出表中的索引。用户可以在此方法的重写实现中检查当前单元格的值，如果需要将当前单元格替换为其他类型和数值，则在此实现中应将期望的类型和数值设置到 CellValue 对象并返回 true。默认情况下，此方法不执行任何操作并返回 false。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 在工作表中创建示例数据
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // 创建 ExportTableOptions 的实例
            ExportTableOptions exportOptions = new ExportTableOptions();

            // 创建用于演示的 CellValue 对象
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // 使用特定参数（第 0 行，第 0 列，CellValue）调用 PreprocessExportedValue
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // 显示方法调用的结果
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // 如有需要，使用处理后的值修改单元格
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // 保存工作簿
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


