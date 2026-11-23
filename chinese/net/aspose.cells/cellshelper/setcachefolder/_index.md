---
title: "CellsHelper.SetCacheFolder"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsHelper 方法。设置可能用作数据缓存的临时文件夹"
type: docs
url: /zh/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

设置可能用作数据缓存的临时文件夹。

```csharp
public static void SetCacheFolder(string cache)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 缓存 | String | 用于可能作为数据缓存的临时文件的文件夹。 |

### 备注

缓存文件通常用于某些功能以提升内存性能，例如将大型数据集保存为 xls 文件，或在单元格模型中使用带文件缓存的内存模式。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodSetCacheFolderWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // 创建用于缓存的临时目录
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // 使用 CellsHelper 设置缓存文件夹
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // 验证缓存文件夹已设置
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // 创建一个简单的工作簿以演示功能
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // 保存工作簿
                workbook.Save("CacheFolderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with cache folder configured.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting cache folder: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


