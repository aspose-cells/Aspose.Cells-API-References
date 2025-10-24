##Enum ReConnectionMethodType
Aspose.Cells.ExternalConnections.ReConnectionMethodType enum. Specifies what the spreadsheet application should do when a connection fails
## ReConnectionMethodType enumeration
Specifies what the spreadsheet application should do when a connection fails.
```csharp
public enum ReConnectionMethodType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Required | `1` | On refresh use the existing connection information and if it ends up being invalid then get updated connection information, if available from the external connection file. |
| Always | `2` | On every refresh get updated connection information from the external connection file, if available, and use that instead of the existing connection information. In this case the data refresh will fail if the external connection file is unavailable. |
| Never | `3` | Never get updated connection information from the external connection file even if it is available and even if the existing connection information is invalid |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionsClassReConnectionMethodTypeDemo
{
public static void Run()
{
try
{
// Demonstrate creating and using ReConnectionMethodType enum values
ReConnectionMethodType method1 = ReConnectionMethodType.Required;
ReConnectionMethodType method2 = ReConnectionMethodType.Always;
ReConnectionMethodType method3 = ReConnectionMethodType.Never;
Console.WriteLine("ReConnectionMethodType values:");
Console.WriteLine($"Required: {(int)method1}");
Console.WriteLine($"Always: {(int)method2}");
Console.WriteLine($"Never: {(int)method3}");
// Show usage in a switch statement
Console.WriteLine("\nDemonstrating switch usage:");
TestConnectionMethod(method1);
TestConnectionMethod(method2);
TestConnectionMethod(method3);
}
catch (Exception ex)
{
Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
}
}
private static void TestConnectionMethod(ReConnectionMethodType method)
{
switch (method)
{
case ReConnectionMethodType.Required:
Console.WriteLine("Using Required reconnection method");
break;
case ReConnectionMethodType.Always:
Console.WriteLine("Using Always reconnection method");
break;
case ReConnectionMethodType.Never:
Console.WriteLine("Using Never reconnection method");
break;
default:
Console.WriteLine("Unknown reconnection method");
break;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
