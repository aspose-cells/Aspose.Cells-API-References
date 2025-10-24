##CellsHelper.CustomImplementationFactory
CellsHelper property. Gets or sets the factory for creating instances with special implementation
## CellsHelper.CustomImplementationFactory property
Gets or sets the factory for creating instances with special implementation.
```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyCustomImplementationFactoryDemo
{
public static void Run()
{
// Create an instance of CustomImplementationFactory
CustomImplementationFactory factory = new CustomImplementationFactory();
// Demonstrate factory methods
MemoryStream memoryStream = factory.CreateMemoryStream();
Console.WriteLine("MemoryStream created without parameters.");
MemoryStream sizedStream = factory.CreateMemoryStream(1024);
Console.WriteLine("MemoryStream created with capacity: 1024");
CultureInfo culture = factory.CreateCultureInfo(1033);
Console.WriteLine($"CultureInfo created: {culture.DisplayName}");
Random random = factory.CreateRandomInstance();
Console.WriteLine($"Random number generated: {random.Next()}");
// Set the factory in CellsHelper
CellsHelper.CustomImplementationFactory = factory;
Console.WriteLine("CustomImplementationFactory set in CellsHelper");
}
}
}
```
### See Also
* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
