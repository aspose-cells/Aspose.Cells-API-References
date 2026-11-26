---
title: "Cells.MemorySetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece la opción de uso de memoria para estas celdas"
type: docs
url: /es/net/aspose.cells/cells/memorysetting/
---
## Cells.MemorySetting property

Obtiene o establece la opción de uso de memoria para estas celdas.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Observaciones

Límites notables y operaciones recomendadas para algunos modos:

| **Mode** | **Remarks** | **Supported** |
| --- | --- | --- |
| MemoryPreference | Los datos de Cells se mantendrán en formato compacto para reducir el costo de memoria. Por otro lado, los datos compactos también pueden causar un mayor costo de tiempo, especialmente al actualizar los datos de las celdas o al acceder a celdas/filas de forma aleatoria | v8.0.0 |
| FileCache | When this mode is used for any worksheet in one workbook, [`Dispose`](../../workbook/dispose/) should be called at the end of work to release all resources such as the temporary files.  Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).  When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects( such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit. | v25.7 |

### Ejemplos

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

### Ver también

* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


