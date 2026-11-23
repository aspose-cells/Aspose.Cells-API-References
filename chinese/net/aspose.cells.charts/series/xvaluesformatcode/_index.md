---
title: "Series.XValuesFormatCode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Series 属性。表示 X Values NumberList 的格式代码"
type: docs
url: /zh/net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

表示 X Values 的 NumberList 的格式代码。

```csharp
public string XValuesFormatCode { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesFormatCodeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(200);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // 设置图表数据源
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // 设置 XValues 格式代码
            chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";

            // 保存工作簿
            workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


