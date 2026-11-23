---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SaveOptions 属性。是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断"
type: docs
url: /zh/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

```csharp
public bool CheckExcelRestriction { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            
            // 禁用 Excel 限制检查
            workbook.Settings.CheckExcelRestriction = false;

            // 访问第一个工作表和单元格
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // 创建一个超过 Excel 正常限制的字符串
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // 将长字符串放入单元格 A1
            cells["A1"].PutValue(longString);

            // 配置保存选项以绕过限制
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // 保存工作簿
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // 加载已保存的文件并禁用限制
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // 验证长字符串已被保留
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### 另请参见

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


