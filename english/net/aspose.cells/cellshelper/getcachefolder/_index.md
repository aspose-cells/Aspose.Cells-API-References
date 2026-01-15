---
title: CellsHelper.GetCacheFolder
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets the folder for temporary files that may be used as data cache
type: docs
url: /net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Gets the folder for temporary files that may be used as data cache.

```csharp
public static string GetCacheFolder()
```

### Return Value

Folder for cache files that has been specified. If it has not been specified, null will be returned and system's temporary path will be used when needed.

### Remarks

Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.

### Examples

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
                // Get the current cache folder path
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Display the cache folder path
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Optionally set a new cache folder (demonstrating the related method)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Verify the change
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Revert to original (optional)
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

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


