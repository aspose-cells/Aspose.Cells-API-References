---
title: "CellsHelper.MergeFiles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Fügt einige große XLS-Dateien zu einer XLS-Datei zusammen"
type: docs
url: /de/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Führt mehrere große XLS-Dateien zu einer XLS-Datei zusammen.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateien | String[] | Die Dateien. |
| cachedFile | String | Die zwischengespeicherte Datei. |
| destFile | String | Die Ziel-Datei. |

### Hinweise

Diese Methode unterstützt nur das Zusammenführen von Daten, Formatierungen und Formeln in die neue Datei. Die zwischengespeicherte Datei wird verwendet, um einige temporäre Daten zu speichern.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // Temporäre Excel-Dateien zum Zusammenführen erstellen
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Beispielarbeitsmappen erstellen
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // Rufen Sie MergeFiles mit String[], String, String-Parametern auf
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Überprüfen Sie die zusammengeführte Datei
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // Bereinige temporäre Dateien
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


