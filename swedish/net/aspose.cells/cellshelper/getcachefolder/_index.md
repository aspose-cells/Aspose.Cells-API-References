---
title: "CellsHelper.GetCacheFolder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar mappen för temporära filer som kan användas som datacache"
type: docs
url: /sv/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Hämtar mappen för temporära filer som kan användas som datacache.

```csharp
public static string GetCacheFolder()
```

### Returvärde

Mapp för cache-filer som har angetts. Om den inte har angetts returneras null och systemets temporära sökväg används vid behov.

### Anmärkningar

Cache-filer används vanligtvis för vissa funktioner för minnesprestanda, såsom att spara stora dataset till xls-fil, eller använda minnesläge med filcache för cellmodellen.

### Exempel

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
                // Hämta den aktuella cache-mappens sökväg
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Visa cache-mappens sökväg
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Ange valfritt en ny cache-mapp (visar den relaterade metoden)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Verifiera ändringen
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Återgå till originalet (valfritt)
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

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


