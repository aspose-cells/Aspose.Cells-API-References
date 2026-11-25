---
title: "CellsHelper.MergeFiles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Unisce alcuni file xls di grandi dimensioni in un file xls"
type: docs
url: /it/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Unisce alcuni file xls di grandi dimensioni in un file xls.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | String[] | I file. |
| cachedFile | String | Il file cache. |
| destFile | String | Il file di destinazione. |

### Osservazioni

Questo metodo supporta solo l'unione di dati, stili e formule nel nuovo file. Il file cache è usato per memorizzare alcuni dati temporanei.

### Esempi

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
            // Crea file Excel temporanei da unire
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Crea cartelle di lavoro di esempio
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
                // Chiama MergeFiles con i parametri String[], String, String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Verifica il file unito
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
                // Pulisci i file temporanei
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


