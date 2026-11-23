---
title: "PivotFilter.GetLabels"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFilter 方法。获取标题过滤器的标签"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

获取标题过滤器的标签。

```csharp
public string[] GetLabels()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建有效的透视表结构
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // 使用正确的参数创建透视表
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // 使用有效参数创建透视过滤器
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // 配置过滤器属性
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // 执行 GetLabels 方法
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


