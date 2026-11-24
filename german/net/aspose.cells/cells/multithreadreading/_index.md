---
title: "Cells.MultiThreadReading"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt an, ob das Zellen-Datenmodell MultiThread-Lesen unterstützen soll, und legt diesen Wert fest. Der Standardwert dieser Eigenschaft ist false"
type: docs
url: /de/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Liest oder legt fest, ob das Zellen‑Datenmodell Multi‑Thread‑Lesen unterstützen soll. Der Standardwert dieser Eigenschaft ist false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Hinweise

Wenn mehrere Threads gleichzeitig Row/Cell-Objekte in dieser Sammlung lesen, sollte diese Eigenschaft auf true gesetzt werden, andernfalls können unerwartete Ergebnisse entstehen. Die Unterstützung von Multi-Thread-Lesen kann die Leistung beim Zugriff auf Row/Cell-Objekte aus dieser Sammlung verringern. Bitte beachten Sie, dass einige Funktionen Multi-Thread-Lesen nicht unterstützen, wie z. B. die Formatierung von Werten (über [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), usw.). Daher können selbst bei auf true gesetzter Eigenschaft diese APIs weiterhin unerwartete Ergebnisse beim Multi-Thread-Lesen liefern.

### Beispiele

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
            
            // Multi-Thread-Lesen aktivieren
            cells.MultiThreadReading = true;

            // Stil für die erste Spalte einrichten
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Zellen mit Beispieldaten füllen
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Threads erstellen, um Zellwerte zu lesen
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

            // Warten, bis alle Threads abgeschlossen sind
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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


