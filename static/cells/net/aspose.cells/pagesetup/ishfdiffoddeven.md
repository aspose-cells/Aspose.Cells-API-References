##PageSetup.IsHFDiffOddEven
PageSetup property. True means that the header/footer of the odd pages is different with odd pages
## PageSetup.IsHFDiffOddEven property
True means that the header/footer of the odd pages is different with odd pages.
```csharp
public bool IsHFDiffOddEven { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsHFDiffOddEvenDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Enable different headers/footers for odd and even pages
pageSetup.IsHFDiffOddEven = true;
// Set different footers for odd and even pages
pageSetup.SetFooter(0, "Odd Page Footer");
pageSetup.SetEvenFooter(0, "Even Page Footer");
// Save the workbook
workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
// Verify the settings by loading the saved file
Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
