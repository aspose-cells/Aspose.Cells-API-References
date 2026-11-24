---
title: "CellsHelper.GetCacheFolder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Ordner für temporäre Dateien zurück, der als Daten-Cache verwendet werden kann"
type: docs
url: /de/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Ermittelt den Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

```csharp
public static string GetCacheFolder()
```

### Rückgabewert

Ordner für Cache-Dateien, der angegeben wurde. Wenn er nicht angegeben wurde, wird null zurückgegeben und bei Bedarf der temporäre Pfad des Systems verwendet.

### Hinweise

Cache-Dateien werden im Allgemeinen für einige Funktionen zur Speicherleistungsoptimierung verwendet, z. B. zum Speichern großer Datensätze in einer xls-Datei oder zur Verwendung des Speichermodus mit Dateicache für das Zellenmodell.

### Beispiele

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
                // Den aktuellen Cache-Ordnerpfad abrufen
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Den Cache-Ordnerpfad anzeigen
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Optional einen neuen Cache-Ordner festlegen (zeigt die zugehörige Methode)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Die Änderung überprüfen
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Zurück zum Original (optional)
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

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


