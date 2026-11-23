---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 属性。获取公式中数组行数据项的分隔符"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

获取公式中数组行数据项的分隔符。

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // 显示 ColumnSeparatorOfFormulaArray 的当前值
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // 为 ColumnSeparatorOfFormulaArray 设置新值
            settings.SetColumnSeparatorOfFormulaArray(';');

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            // 使用 SetArrayFormula 创建带自定义分隔符的数组公式
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // 计算公式
            workbook.CalculateFormula();

            // 显示结果
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // 保存工作簿
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


