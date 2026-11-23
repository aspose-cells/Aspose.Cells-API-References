---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 属性。获取公式中数组数据行的分隔符"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

获取公式中数组数据行的分隔符。

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // 显示公式数组的默认行分隔符
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // 为公式数组设置新的行分隔符
            settings.SetRowSeparatorOfFormulaArray(';');

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            // 在工作表中创建数组公式
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // 计算公式
            workbook.CalculateFormula();

            // 保存工作簿
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


