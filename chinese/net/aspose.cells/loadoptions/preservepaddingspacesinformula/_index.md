---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LoadOptions 属性。指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。"
type: docs
url: /zh/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### 备注

使用此选项从模板文件加载工作簿后，[`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) 将被设置为与此属性相同的值。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 启用在公式中保留填充空格
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // 访问第一个工作表并设置带有填充空格的公式
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // 使用 PreservePaddingSpacesInFormula 选项保存并重新加载工作簿
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // 验证重新加载后公式保留了空格
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### 另请参见

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


