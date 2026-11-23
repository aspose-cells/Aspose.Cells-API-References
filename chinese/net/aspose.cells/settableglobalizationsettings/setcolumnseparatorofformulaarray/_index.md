---
title: "SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置公式中数组行数据项的分隔符"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

设置公式中数组行数据项的分隔符。

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | 字符 | 指定的分隔符 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


