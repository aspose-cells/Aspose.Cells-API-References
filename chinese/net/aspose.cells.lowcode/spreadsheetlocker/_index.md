---
title: "类 SpreadsheetLocker"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.LowCode.SpreadsheetLocker 类。低代码 API 用于锁定电子表格文件"
type: docs
url: /zh/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

用于锁定电子表格文件的低代码 API。

```csharp
public class SpreadsheetLocker
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | 使用指定设置锁定电子表格文件。 |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | 使用指定设置锁定电子表格文件。 |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | 使用指定设置锁定电子表格文件。 |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | 使用指定设置锁定电子表格文件。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // 使用 SpreadsheetLocker 保护工作簿
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


