---
title: "Cells.MemorySetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger minnesanvändningsalternativet för dessa celler"
type: docs
url: /sv/net/aspose.cells/cells/memorysetting/
---
## Cells.MemorySetting property

Hämtar eller anger minnesanvändningsalternativet för dessa celler.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Anmärkningar

Anmärkningsvärda begränsningar och rekommenderade operationer för vissa lägen:

| **Läge** | **Anmärkningar** | **Stöds** |
| --- | --- | --- |
| MemoryPreference | Cells data kommer att hållas i kompakt format för att minska minneskostnaden. Å andra sidan kan den kompakta datan också medföra högre tidskostnad, särskilt vid uppdatering av celldata eller vid slumpmässig åtkomst till celler/rader. | v8.0.0 |
| FileCache | When this mode is used for any worksheet in one workbook, [`Dispose`](../../workbook/dispose/) should be called at the end of work to release all resources such as the temporary files.  Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).  When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects( such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit. | v25.7 |

### Exempel

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMemorySettingDemo
    {
        private static Workbook workbook;
        private static Cells cells;

        private static void ThreadLoop()
        {
            for (int i = 0; i < 3; i++)
            {
                cells[i, 0].PutValue($"Thread {Thread.CurrentThread.ManagedThreadId} - {i}");
            }
        }

        public static void Run()
        {
            workbook = new Workbook();
            cells = workbook.Worksheets[0].Cells;

            Console.WriteLine("Testing MultiThreadReading with Normal memory setting...");
            cells.MemorySetting = MemorySetting.Normal;
            
            Thread thread1 = new Thread(ThreadLoop);
            Thread thread2 = new Thread(ThreadLoop);
            
            thread1.Start();
            thread2.Start();
            thread1.Join();
            thread2.Join();

            Console.WriteLine("Testing MultiThreadReading with MemoryPreference setting...");
            cells.MemorySetting = MemorySetting.MemoryPreference;
            
            thread1 = new Thread(ThreadLoop);
            thread2 = new Thread(ThreadLoop);
            
            thread1.Start();
            thread2.Start();
            thread1.Join();
            thread2.Join();

            Console.WriteLine("Demo finished. Workbook saved to output.xlsx");
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


