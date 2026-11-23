---
title: "WorkbookDesigner.SortDataSource"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookDesigner 属性。指示是否对数据源进行排序"
type: docs
url: /zh/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

指示是否对数据源进行排序。

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### 备注

注意：此属性现已过时。自2026年10月起，此属性将在12个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。如果智能标记包含升序和降序参数，Json 数据源将被排序。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // 创建一个包含未排序数据的示例 DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // 以未排序的顺序添加示例数据
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // 创建一个带有智能标记的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 在工作表中设置智能标记
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // 创建 WorkbookDesigner 实例
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // 显示初始 SortDataSource 值
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // 设置未排序的数据源
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // 保存未排序的结果
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // 创建一个用于排序演示的新工作簿
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // 创建启用排序的新 WorkbookDesigner
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // 保存已排序的结果
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
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

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


