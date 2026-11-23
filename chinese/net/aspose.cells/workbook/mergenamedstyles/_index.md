---
title: "Workbook.MergeNamedStyles"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 方法。合并来自另一个 Excel 文件的命名样式"
type: docs
url: /zh/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

合并来自另一个 Excel 文件的命名样式。

```csharp
public void MergeNamedStyles(Workbook source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 源 | Workbook | 另一个文件 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // 创建目标工作簿（将接收命名样式的工作簿）
            using (Workbook targetWorkbook = new Workbook())
            {
                // 向目标工作簿添加一些数据以提供上下文
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // 创建源工作簿（包含要合并的命名样式的工作簿）
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // 向源工作簿添加一些数据以提供上下文
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // 将 sourceWorkbook 中的命名样式合并到 targetWorkbook
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // 保存生成的工作簿
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### 另请参见

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


