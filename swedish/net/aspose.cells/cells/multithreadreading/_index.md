---
title: "Cells.MultiThreadReading"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger om cellernas datamodell ska stödja MultiThread-läsning. Standardvärdet för denna egenskap är false"
type: docs
url: /sv/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Hämtar eller anger om cellernas datamodell ska stödja Multi-Thread läsning. Standardvärdet för denna egenskap är falskt.

```csharp
public bool MultiThreadReading { get; set; }
```

### Anmärkningar

Om det finns flera trådar som läser Row/Cell-objekt i denna samling samtidigt, bör denna egenskap sättas till true, annars kan oväntade resultat uppstå. Stöd för Multi-Thread-läsning kan försämra prestandan vid åtkomst av Row/Cell-objekt från denna samling. Observera att vissa funktioner inte kan stödja Multi-Thread-läsning, såsom formatering av värden (genom [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), etc.). Så även om denna egenskap är satt till true, kan dessa API:er fortfarande ge oväntade resultat för Multi-Thread-läsning.

### Exempel

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
            
            // Aktivera multi-thread-läsning
            cells.MultiThreadReading = true;

            // Ställ in stil för den första kolumnen
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Fyll celler med exempeldata
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Skapa trådar för att läsa cellvärden
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

            // Vänta på att alla trådar ska slutföras
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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


