---
title: "SaveOptions.CachedFileFolder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können"
type: docs
url: /de/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

```csharp
public string CachedFileFolder { get; set; }
```

### Hinweise

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [`GetCacheFolder`](../../cellshelper/getcachefolder/). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache-Datei verwendet.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Speicheroptionen mit Cache-Ordner festlegen
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Speichere die Arbeitsmappe
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


