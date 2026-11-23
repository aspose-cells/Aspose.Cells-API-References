---
title: "LowCodeLoadOptions.InputFile"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeLoadOptions 属性。获取和设置模板的文件路径（如有需要）"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

获取并设置模板的文件（如有需要包括路径）。

```csharp
public string InputFile { get; set; }
```

### 备注

当为此属性设置非 null 且非空的路径时，先前为 [`InputStream`](../inputstream/) 设置的值将被忽略。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // 创建并保存示例模板文件
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // 初始化 LowCodeLoadOptions 并演示 InputFile 属性
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // 设置 InputFile 属性以使用我们的模板
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // 使用指定的模板文件加载工作簿
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // 修改已加载的模板
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // 保存已修改的工作簿
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


