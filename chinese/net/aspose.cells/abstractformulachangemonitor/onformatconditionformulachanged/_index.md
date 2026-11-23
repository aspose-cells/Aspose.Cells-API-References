---
title: "AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractFormulaChangeMonitor 方法。当 FormatCondition 的公式被更改时将触发的事件"
type: docs
url: /zh/net/aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/
---
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method

当 FormatCondition 的公式更改时将触发的事件。

```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fc | FormatCondition | 其公式已更改的 FormatCondition 对象 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // 创建条件格式
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // 创建格式条件
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style = workbook.CreateStyle();
            fc.Style.Font.Color = System.Drawing.Color.Red;

            // 创建自定义监视器
            var monitor = new CustomFormulaChangeMonitor();

            try
            {
                // 调用 OnFormatConditionFormulaChanged 方法
                monitor.OnFormatConditionFormulaChanged(fc);

                Console.WriteLine("Method executed successfully with FormatCondition parameter");

                // 将条件格式应用于一个范围
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 2;
                area.EndColumn = 0;
                fcs.AddArea(area);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnFormatConditionFormulaChanged method: {ex.Message}");
            }

            workbook.Save("MethodOnFormatConditionFormulaChangedDemo.xlsx");
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            Console.WriteLine($"Format condition formula changed. Type: {fc.Type}, Formula1: {fc.Formula1}, Formula2: {fc.Formula2}");
        }
    }

}
```

### 另请参见

* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


