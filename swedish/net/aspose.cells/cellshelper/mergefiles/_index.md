---
title: "CellsHelper.MergeFiles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Slår ihop några stora xls-filer till en xls-fil"
type: docs
url: /sv/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Slår samman några stora xls‑filer till en xls‑fil.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filer | String[] | Filerna. |
| cachedFile | String | Den cachade filen. |
| destFile | String | Destfilen. |

### Anmärkningar

Denna metod stöder endast sammanslagning av data, stil och formler till den nya filen. Den cachade filen används för att lagra viss temporär data.

### Exempel

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
            // Skapa tillfälliga Excel-filer för sammanslagning
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Skapa exempelarbetsböcker
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
                // Anropa MergeFiles med parametrarna String[], String, String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Verifiera den sammanslagna filen
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
                // Rensa temporära filer
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


