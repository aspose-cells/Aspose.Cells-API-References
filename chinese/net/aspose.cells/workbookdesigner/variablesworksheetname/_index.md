---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookDesigner 属性。获取和设置包含变量智能标记的工作表名称"
type: docs
url: /zh/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

获取和设置包含变量智能标记的工作表名称。

```csharp
public string VariablesWorksheetName { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();

                // 添加一个名为 "Variables" 的工作表以演示该属性
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // 创建 WorkbookDesigner 实例
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // 显示当前 VariablesWorksheetName 值
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // 为 VariablesWorksheetName 设置新值
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // 添加另一个带有智能标记的工作表
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // 处理智能标记
                designer.Process();

                // 保存工作簿
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
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


