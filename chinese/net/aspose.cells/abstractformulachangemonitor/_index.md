---
title: "类 AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.AbstractFormulaChangeMonitor 类。用于在特定操作期间监视用户跟踪公式的更改"
type: docs
url: /zh/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

用于在特定操作期间监视用户跟踪公式的更改。

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | 当单元格中的公式更改时将触发的事件。 |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | 当 FormatCondition 的公式更改时将触发的事件。 |

### 备注

例如，在删除/插入单元格范围时，其他单元格的公式可能会因引用移动而更改。请注意，监视器中的方法可能会针对包含公式的同一对象被调用多次。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // 在单元格中设置一些公式
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // 插入会触发公式更改的行
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


