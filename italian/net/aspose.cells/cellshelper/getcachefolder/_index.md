---
title: "CellsHelper.GetCacheFolder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellsHelper. Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati"
type: docs
url: /it/net/aspose.cells/cellshelper/getcachefolder/
---
## CellsHelper.GetCacheFolder method

Ottiene la cartella per i file temporanei che possono essere usati come cache dei dati.

```csharp
public static string GetCacheFolder()
```

### Valore di ritorno

Cartella per i file di cache specificata. Se non è stata specificata, verrà restituito null e verrà usato il percorso temporaneo del sistema quando necessario.

### Osservazioni

I file di cache sono generalmente usati per alcune funzionalità relative alle prestazioni di memoria, come il salvataggio di grandi set di dati in file xls, o l'uso della modalità memoria con cache di file per il modello di celle.

### Esempi

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
                // Ottieni il percorso corrente della cartella della cache
                string cacheFolder = CellsHelper.GetCacheFolder();

                // Visualizza il percorso della cartella della cache
                Console.WriteLine("Current cache folder path: " + cacheFolder);

                // Facoltativamente imposta una nuova cartella della cache (dimostrando il metodo correlato)
                string newCacheFolder = @"C:\Temp\AsposeCache";
                CellsHelper.SetCacheFolder(newCacheFolder);

                // Verifica la modifica
                string updatedCacheFolder = CellsHelper.GetCacheFolder();
                Console.WriteLine("Updated cache folder path: " + updatedCacheFolder);

                // Ripristina l'originale (opzionale)
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

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


