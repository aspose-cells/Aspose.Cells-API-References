##WriteProtection.Author
WriteProtection property. Gets and sets the author
## WriteProtection.Author property
Gets and sets the author.
```csharp
public string Author { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WriteProtectionPropertyAuthorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WorkbookSettings settings = workbook.Settings;
WriteProtection writeProtection = settings.WriteProtection;
// Demonstrate Author property usage
writeProtection.Author = "John Doe";
writeProtection.Password = "password123";
Console.WriteLine("Write protection author: " + writeProtection.Author);
Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);
workbook.Save("WriteProtectionDemo.xlsx");
}
}
}
```
### See Also
* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
