---
title: "CellsHelper.SetCacheFolder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Imposta la cartella per i file temporanei che possono essere usati come cache dei dati"
type: docs
url: /it/net/aspose.cells/cellshelper/setcachefolder/
---
## CellsHelper.SetCacheFolder method

Imposta la cartella per i file temporanei che possono essere usati come cache dei dati.

```csharp
public static void SetCacheFolder(string cache)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cache | String | Cartella per i file temporanei che possono essere usati come cache dei dati. |

### Osservazioni

I file di cache sono generalmente usati per alcune funzionalità relative alle prestazioni di memoria, come il salvataggio di grandi set di dati in file xls, o l'uso della modalità memoria con cache di file per il modello di celle.

### Esempi

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
                // Crea una directory temporanea per la cache
                string tempCacheFolder = Path.Combine(Path.GetTempPath(), "AsposeCellsCache");
                Directory.CreateDirectory(tempCacheFolder);

                // Imposta la cartella della cache usando CellsHelper
                CellsHelper.SetCacheFolder(tempCacheFolder);

                // Verifica che la cartella della cache sia stata impostata
                string currentCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine($"Cache folder set to: {currentCacheFolder}");

                // Crea una cartella di lavoro semplice per dimostrare la funzionalità
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Cache folder demonstration";
                worksheet.Cells["A2"].Value = $"Using cache at: {currentCacheFolder}";

                // Salva la cartella di lavoro
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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


