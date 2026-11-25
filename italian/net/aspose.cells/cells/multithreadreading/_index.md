---
title: "Cells.MultiThreadReading"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene o imposta se il modello dati delle celle deve supportare la lettura MultiThread. Il valore predefinito di questa proprietà è false"
type: docs
url: /it/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Ottiene o imposta se il modello dati delle celle deve supportare la lettura Multi-Thread. Il valore predefinito di questa proprietà è false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Osservazioni

Se ci sono più thread che leggono oggetti Row/Cell in questa collezione contemporaneamente, questa proprietà dovrebbe essere impostata su true, altrimenti potrebbero verificarsi risultati inattesi. Supportare la lettura Multi-Thread può degradare le prestazioni nell'accesso agli oggetti Row/Cell di questa collezione. Si noti che alcune funzionalità non possono supportare la lettura Multi-Thread, come la formattazione dei valori (tramite [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), ecc.). Pertanto, anche se questa proprietà è impostata su true, quelle API potrebbero comunque produrre risultati inattesi per la lettura Multi-Thread.

### Esempi

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Abilita la lettura multi-thread
            cells.MultiThreadReading = true;

            // Configura lo stile per la prima colonna
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Popola le celle con dati di esempio
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Crea thread per leggere i valori delle celle
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // Attendi il completamento di tutti i thread
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


