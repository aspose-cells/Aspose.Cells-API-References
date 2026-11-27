---
title: "CellsHelper.SetCacheFolder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Anger mappen för temporära filer som kan användas som datacache"
type: docs
url: /sv/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Ställer in mappen för temporära filer som kan användas som datacache.

```csharp
public static void SetCacheFolder(string cache)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cache | String | Mapp för temporära filer som kan användas som datacache. |

### Anmärkningar

Cache-filer används vanligtvis för vissa funktioner för minnesprestanda, såsom att spara stora dataset till xls-fil, eller använda minnesläge med filcache för cellmodellen.

### Exempel

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
                // Skapa en temporär katalog för cache
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Ange cache-mappen med CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Verifiera att cache-mappen har ställts in
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Skapa en enkel arbetsbok för att demonstrera funktionaliteten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Spara arbetsboken
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

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


