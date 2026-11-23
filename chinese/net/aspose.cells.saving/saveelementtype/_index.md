---
title: "枚举 SaveElementType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Saving.SaveElementType 枚举。表示应该保存哪种类型的元素。"
type: docs
url: /zh/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

表示应该保存哪种类型的元素。

```csharp
public enum SaveElementType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| All | `251658239` | 所有数据。 |
| Chart | `256` | 仅图表。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 添加一些示例数据以演示保存
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // 创建图表以演示图表保存元素类型
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // 演示使用 SaveElementType 枚举值
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // 保存工作簿及所有元素
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


