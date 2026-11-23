---
title: "SpreadsheetConverter.Process"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SpreadsheetConverter 方法。将给定的模板文件在电子表格文件格式之间进行转换"
type: docs
url: /zh/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

将给定的模板文件在电子表格文件格式之间进行转换。

```csharp
public static void Process(string templateFile, string resultFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | String | 待转换的模板文件 |
| resultFile | String | 生成的文件 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### 另请参见

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

在不同电子表格文件格式之间进行转换。

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | 输入和加载的选项 |
| saveOptions | LowCodeSaveOptions | 输出和保存的选项 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // 使用输入文件创建加载选项
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // 使用输出文件创建保存选项
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // 执行转换
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### 另请参见

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


