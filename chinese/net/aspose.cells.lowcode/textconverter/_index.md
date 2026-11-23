---
title: "类 TextConverter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.TextConverter 类。用于在基于文本的格式（csv、tsv、dif...）与其他电子表格文件格式之间转换的转换器"
type: docs
url: /zh/net/aspose.cells.lowcode/textconverter/
---
## TextConverter class

用于在基于文本的格式（csv、tsv、dif 等）与其他电子表格文件格式之间转换的转换器。

```csharp
public class TextConverter
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | 在基于文本的格式与其他电子表格文件格式之间转换文件格式 |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | 在基于文本的文件与其他格式之间转换给定的模板文件。 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterDemo
    {
        public static void Process(string inputFile, string outputFile)
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            string[] lines = File.ReadAllLines(inputFile);
            for (int i = 0; i < lines.Length; i++)
            {
                string[] cells = lines[i].Split(',');
                for (int j = 0; j < cells.Length; j++)
                {
                    worksheet.Cells[i, j].PutValue(cells[j]);
                }
            }

            workbook.Save(outputFile, SaveFormat.Xlsx);
        }
    }

    public class LowCodeClassTextConverterDemo
    {
        public static void Run()
        {
            TextConverter.Process("template.csv", "res.xlsx");
            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


