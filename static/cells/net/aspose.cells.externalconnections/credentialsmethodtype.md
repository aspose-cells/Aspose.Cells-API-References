##Enum CredentialsMethodType
Aspose.Cells.ExternalConnections.CredentialsMethodType enum. Specifies Credentials method used for server access
## CredentialsMethodType enumeration
Specifies Credentials method used for server access.
```csharp
public enum CredentialsMethodType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Integrated | `0` | Integrated Authentication |
| None | `1` | No Credentials |
| Prompt | `2` | Prompt Credentials |
| Stored | `3` | Stored Credentials |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionsClassCredentialsMethodTypeDemo
{
public static void Run()
{
try
{
// Demonstrate all enum values of CredentialsMethodType
Console.WriteLine("Available CredentialsMethodType values:");
foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
{
Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
}
// Show practical usage with a specific value
CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
Console.WriteLine($"\nSelected method: {selectedMethod}");
// Demonstrate switch usage
switch (selectedMethod)
{
case CredentialsMethodType.Integrated:
Console.WriteLine("Using integrated authentication");
break;
case CredentialsMethodType.None:
Console.WriteLine("No credentials will be used");
break;
case CredentialsMethodType.Prompt:
Console.WriteLine("User will be prompted for credentials");
break;
case CredentialsMethodType.Stored:
Console.WriteLine("Using stored credentials");
break;
}
}
catch (Exception ex)
{
Console.WriteLine($"Error demonstrating CredentialsMethodType: {ex.Message}");
}
}
private static string GetMethodDescription(CredentialsMethodType method)
{
return method switch
{
CredentialsMethodType.Integrated => "Integrated Authentication",
CredentialsMethodType.None => "No Credentials",
CredentialsMethodType.Prompt => "Prompt Credentials",
CredentialsMethodType.Stored => "Stored Credentials",
_ => "Unknown method"
};
}
}
}
```
### See Also
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)
