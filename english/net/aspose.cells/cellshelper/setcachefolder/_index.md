---
title: CellsHelper.SetCacheFolder
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Sets the folder for temporary files that may be used as data cache
type: docs
url: /net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Sets the folder for temporary files that may be used as data cache.

```csharp
public static void SetCacheFolder(string cache)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cache | String | Folder for for temporary files that may be used as data cache. |

### Remarks

Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.

### Examples

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
                // Create a temporary directory for cache
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Set the cache folder using CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Verify the cache folder was set
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Create a simple workbook to demonstrate functionality
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Save the workbook
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

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


