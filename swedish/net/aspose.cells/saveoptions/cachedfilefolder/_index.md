---
title: "SaveOptions.CachedFileFolder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Mappen för temporära filer som kan användas som datacache"
type: docs
url: /sv/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

Mappen för temporära filer som kan användas som datacache.

```csharp
public string CachedFileFolder { get; set; }
```

### Anmärkningar

Om mappen inte har angetts är standardvärdet för den [`GetCacheFolder`](../../cellshelper/getcachefolder/). Om dess standardvärde är null eller tomt, eller har angetts som null eller tomt, kommer ingen cachefil att användas när arbetsboken sparas.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Ställ in sparalternativ med cachefilsmapp
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Spara arbetsboken
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


