##Cells.MemorySetting
Cells property. Gets or sets the memory usage option for this cells
## Cells.MemorySetting property
Gets or sets the memory usage option for this cells.
```csharp
public MemorySetting MemorySetting { get; set; }
```
### Remarks
Notable limits and recommended operations for some modes:
| **Mode** | **Remarks** | **Supported** |
| --- | --- | --- |
| MemoryPreference | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
| FileCache | When this mode is used for any worksheet in one workbook, [`Dispose`](../../workbook/dispose/) should be called at the end of work to release all resources such as the temporary files.  Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).  When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects( such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit. | v25.7 |
### Examples
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
### See Also
* enum [MemorySetting](../../memorysetting/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
