##CellsHelper.IsCloudPlatform
CellsHelper property. Please set this property True when running on a cloud platform such as Azure AWSLambda etc
## CellsHelper.IsCloudPlatform property
Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,
```csharp
public static bool IsCloudPlatform { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyIsCloudPlatformDemo
{
public static void Run()
{
// Set IsCloudPlatform property
CellsHelper.IsCloudPlatform = true;
// Demonstrate the property usage
Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);
// Show how it affects other operations (example)
if (CellsHelper.IsCloudPlatform)
{
Console.WriteLine("Running in cloud environment - using cloud-specific settings");
CellsHelper.StartupPath = "/cloud_storage/aspose/cells";
}
else
{
Console.WriteLine("Running in local environment");
CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
}
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
