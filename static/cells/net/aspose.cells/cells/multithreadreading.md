##Cells.MultiThreadReading
Cells property. Gets or sets whether the cells data model should support MultiThread reading. Default value of this property is false
## Cells.MultiThreadReading property
Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.
```csharp
public bool MultiThreadReading { get; set; }
```
### Remarks
If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.
### Examples
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
// Enable multi-thread reading
cells.MultiThreadReading = true;
// Setup style for the first column
Style style = wb.CreateStyle();
style.Custom = "yyyy-mm-dd";
StyleFlag sf = new StyleFlag();
sf.All = true;
cells.Columns[0].ApplyStyle(style, sf);
// Populate cells with sample data
int rowCount = 1000;
for (int i = 0; i < rowCount; i++)
{
cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
}
// Create threads to read cell values
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
// Wait for all threads to complete
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
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
