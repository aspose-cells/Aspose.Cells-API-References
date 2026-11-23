---
title: "CellsHelper.GetCacheFolder"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsHelper 方法。获取可能用作数据缓存的临时文件夹"
type: docs
url: /zh/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

获取可能用作数据缓存的临时文件夹。

```csharp
public static string GetCacheFolder()
```

### 返回值

已指定的缓存文件夹。如果未指定，将返回 null，并在需要时使用系统的临时路径。

### 备注

缓存文件通常用于某些功能以提升内存性能，例如将大型数据集保存为 xls 文件，或在单元格模型中使用带文件缓存的内存模式。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetCacheFolderDemo
    {
        public static void Run()
        {
            try
            {
                // 获取当前缓存文件夹路径
                string cacheFolder = CellsHelper.GetCacheFolder();

                // 显示缓存文件夹路径
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // 可选地设置一个新的缓存文件夹（演示相关方法）
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // 验证更改
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // 恢复到原始状态（可选）
                CellsHelper.SetCacheFolder(cacheFolder);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with cache folder: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


