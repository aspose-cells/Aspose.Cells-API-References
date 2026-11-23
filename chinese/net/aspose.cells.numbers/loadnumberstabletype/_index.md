---
title: "枚举 LoadNumbersTableType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Numbers.LoadNumbersTableType 枚举。指示当工作表中包含多个表时的加载表类型"
type: docs
url: /zh/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

指示当某些表位于同一工作表中时的加载表类型。

```csharp
public enum LoadNumbersTableType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建一个新的工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 NumbersLoadOptions 的实例
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // 设置 LoadNumbersTableType 属性
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // 使用指定的加载选项加载 Numbers 文件
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // 将工作簿保存为 Excel 文件
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


