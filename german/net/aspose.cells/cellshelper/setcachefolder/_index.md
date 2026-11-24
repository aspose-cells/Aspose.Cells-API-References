---
title: "CellsHelper.SetCacheFolder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Legt den Ordner für temporäre Dateien fest, die als Daten-Cache verwendet werden können"
type: docs
url: /de/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Setzt den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

```csharp
public static void SetCacheFolder(string cache)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Cache | String | Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |

### Hinweise

Cache-Dateien werden im Allgemeinen für einige Funktionen zur Speicherleistungsoptimierung verwendet, z. B. zum Speichern großer Datensätze in einer xls-Datei oder zur Verwendung des Speichermodus mit Dateicache für das Zellenmodell.

### Beispiele

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
                // Erstellen Sie ein temporäres Verzeichnis für den Cache
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Legen Sie den Cache-Ordner mit CellsHelper fest
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Überprüfen Sie, ob der Cache-Ordner festgelegt wurde
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Erstellen Sie eine einfache Arbeitsmappe, um die Funktionalität zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


