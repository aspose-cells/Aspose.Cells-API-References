##AbstractLowCodeLoadOptionsProvider.Current
AbstractLowCodeLoadOptionsProvider property. Gets the load options from which to load data of currently processed part
## AbstractLowCodeLoadOptionsProvider.Current property
Gets the load options from which to load data of currently processed part.
```csharp
public abstract LowCodeLoadOptions Current { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.Collections;
public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
{
public static void Run()
{
string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
// Initialize custom provider with our load options
CustomProvider provider = new CustomProvider(files);
int counter = 1;
while (provider.MoveNext())
{
// Access Current property to get active load options
Console.WriteLine($"Processing set {counter}");
// Create workbook using current load options' input file/stream
Workbook workbook;
if (provider.Current.InputFile != null)
{
workbook = new Workbook(provider.Current.InputFile);
}
else if (provider.Current.InputStream != null)
{
workbook = new Workbook(provider.Current.InputStream);
}
else
{
workbook = new Workbook();
}
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate option impact removed due to missing property
worksheet.Cells["A1"].Value = "Sample Value";
// Save result
workbook.Save($"CurrentDemo_{counter}.xlsx");
counter++;
}
}
}
// Custom provider implementation with IDisposable
public class CustomProvider : AbstractLowCodeLoadOptionsProvider
{
public IEnumerator fileIter;
public CustomProvider(string[] files)
{
fileIter = files.GetEnumerator();
current = new LowCodeLoadOptions();
}
private LowCodeLoadOptions current;
public override LowCodeLoadOptions Current => current;
public override bool MoveNext()
{
if (fileIter.MoveNext())
{
current = new LowCodeLoadOptions();
current.InputFile = fileIter.Current.ToString();
return true;
}
return false;
}
public override void Finish(LowCodeLoadOptions part)
{
base.Finish(part);
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
