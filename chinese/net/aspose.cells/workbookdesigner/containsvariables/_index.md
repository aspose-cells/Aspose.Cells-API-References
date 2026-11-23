---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookDesigner 属性。指示第一个工作表是否包含自定义变量"
type: docs
url: /zh/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

指示第一个工作表是否包含自定义变量。

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### 备注

注意：此成员现已过时。请改用 WorkbookDesigner.VariablesWorksheetName 属性。该属性将在自 2025 年 9 月起的 3 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建示例工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以使示例更有意义
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 创建 WorkbookDesigner 实例
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // 显示 ContainsVariables 属性的当前值
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // 将 ContainsVariables 属性设置为 true
                designer.ContainsVariables = true;

                // 显示更新后的值
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // 保存结果
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
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


